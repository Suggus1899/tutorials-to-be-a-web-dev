# Día 3: useEffect Básico

En este día aprenderás el hook useEffect.

## Contenido
- Efectos secundarios
- Sintaxis de useEffect
- Array de dependencias
- Cuándo se ejecuta

## Tareas

### Tarea 1: Primer useEffect
Ejecuta código después del render:
```jsx
import { useState, useEffect } from 'react';

function Component() {
  const [count, setCount] = useState(0);
  
  useEffect(() => {
    document.title = `Count: ${count}`;
  }, [count]);
  
  return <button onClick={() => setCount(count + 1)}>{count}</button>;
}
```

### Tarea 2: Fetch de datos
Obtén datos de una API:
```jsx
useEffect(() => {
  async function fetchData() {
    const res = await fetch('/api/users');
    const data = await res.json();
    setUsers(data);
  }
  fetchData();
}, []);
```

### Tarea 3: Dependencias
Entiende las dependencias:
- [] → ejecuta solo al montar
- [value] → ejecuta cuando value cambia
- sin array → ejecuta en cada render

## Ejercicios Adicionales
- Practica con múltiples useEffect
- Experimenta con APIs públicas
