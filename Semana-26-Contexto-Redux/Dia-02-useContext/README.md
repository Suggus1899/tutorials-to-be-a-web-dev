# Día 2: useContext Hook

En este día aprenderás patrones avanzados con Context.

## Contenido
- Custom provider
- Context con reducer
- Separar state y dispatch
- Mejores prácticas

## Tareas

### Tarea 1: Custom Provider
Crea un provider encapsulado:
```jsx
function AuthProvider({ children }) {
  const [user, setUser] = useState(null);
  
  const login = (userData) => setUser(userData);
  const logout = () => setUser(null);
  
  return (
    <AuthContext.Provider value={{ user, login, logout }}>
      {children}
    </AuthContext.Provider>
  );
}
```

### Tarea 2: Custom hook
Crea hook para el contexto:
```jsx
function useAuth() {
  const context = useContext(AuthContext);
  if (!context) {
    throw new Error('useAuth must be used within AuthProvider');
  }
  return context;
}
```

### Tarea 3: Context con useReducer
Combina Context con reducer:
```jsx
function CartProvider({ children }) {
  const [state, dispatch] = useReducer(cartReducer, initialState);
  return (
    <CartContext.Provider value={{ state, dispatch }}>
      {children}
    </CartContext.Provider>
  );
}
```

## Ejercicios Adicionales
- Implementa carrito de compras
- Practica con optimización de contextos
