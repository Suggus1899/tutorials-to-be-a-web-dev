# Día 6: Rutas Protegidas

En este día aprenderás a proteger rutas.

## Contenido
- Rutas que requieren autenticación
- Componente ProtectedRoute
- Redirect después de login
- Persistir estado de auth

## Tareas

### Tarea 1: Componente ProtectedRoute
Crea wrapper de protección:
```jsx
function ProtectedRoute({ children }) {
  const { user } = useAuth();
  
  if (!user) {
    return <Navigate to="/login" replace />;
  }
  
  return children;
}
```

### Tarea 2: Aplicar a rutas
Protege rutas:
```jsx
<Route 
  path="/dashboard" 
  element={
    <ProtectedRoute>
      <Dashboard />
    </ProtectedRoute>
  } 
/>
```

### Tarea 3: Redirect al login
Guarda la ruta intentada:
```jsx
function ProtectedRoute({ children }) {
  const { user } = useAuth();
  const location = useLocation();
  
  if (!user) {
    return <Navigate to="/login" state={{ from: location }} replace />;
  }
  return children;
}

// En login, redirige de vuelta
const from = location.state?.from?.pathname || '/dashboard';
navigate(from, { replace: true });
```

## Ejercicios Adicionales
- Implementa rutas por rol
- Practica con multiple auth levels
