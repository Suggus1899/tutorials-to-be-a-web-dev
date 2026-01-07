# Día 6: Custom Hooks

En este día aprenderás a crear hooks personalizados.

## Contenido
- Por qué custom hooks
- Cómo crearlos
- Patrones comunes
- Compartir lógica

## Tareas

### Tarea 1: Primer custom hook
Crea useCounter:
```jsx
function useCounter(initial = 0) {
  const [count, setCount] = useState(initial);
  const increment = () => setCount(c => c + 1);
  const decrement = () => setCount(c => c - 1);
  const reset = () => setCount(initial);
  return { count, increment, decrement, reset };
}

// Uso
const { count, increment } = useCounter(10);
```

### Tarea 2: useFetch
Crea hook para fetch:
```jsx
function useFetch(url) {
  const [data, setData] = useState(null);
  const [loading, setLoading] = useState(true);
  const [error, setError] = useState(null);
  
  useEffect(() => { /* fetch logic */ }, [url]);
  
  return { data, loading, error };
}
```

### Tarea 3: useLocalStorage
Crea hook para localStorage:
```jsx
function useLocalStorage(key, initialValue) {
  const [value, setValue] = useState(() => {
    const stored = localStorage.getItem(key);
    return stored ? JSON.parse(stored) : initialValue;
  });
  // ... save to localStorage on change
  return [value, setValue];
}
```

## Ejercicios Adicionales
- Crea useToggle
- Crea useDebounce
