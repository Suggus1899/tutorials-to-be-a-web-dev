# Día 5: Hooks Avanzados

En este día aprenderás hooks adicionales.

## Contenido
- useRef
- useMemo
- useCallback
- Cuándo usarlos

## Tareas

### Tarea 1: useRef
Referencia elementos DOM:
```jsx
const inputRef = useRef(null);

function focusInput() {
  inputRef.current.focus();
}

return <input ref={inputRef} />;
```

### Tarea 2: useMemo
Memoriza cálculos costosos:
```jsx
const sortedItems = useMemo(() => {
  return items.sort((a, b) => a.name.localeCompare(b.name));
}, [items]);
```

### Tarea 3: useCallback
Memoriza funciones:
```jsx
const handleClick = useCallback(() => {
  console.log('clicked', count);
}, [count]);
```

## Ejercicios Adicionales
- Practica con useRef para valores persistentes
- Experimenta optimizando renders
