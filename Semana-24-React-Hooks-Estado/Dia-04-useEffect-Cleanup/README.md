# Día 4: useEffect Cleanup

En este día aprenderás sobre cleanup en useEffect.

## Contenido
- Función de cleanup
- Suscripciones y timers
- Prevenir memory leaks
- AbortController

## Tareas

### Tarea 1: Cleanup básico
Limpia recursos:
```jsx
useEffect(() => {
  const timer = setInterval(() => {
    console.log('tick');
  }, 1000);
  
  // Cleanup
  return () => clearInterval(timer);
}, []);
```

### Tarea 2: Cancelar peticiones
Usa AbortController:
```jsx
useEffect(() => {
  const controller = new AbortController();
  
  fetch('/api/data', { signal: controller.signal })
    .then(res => res.json())
    .then(setData)
    .catch(err => {
      if (err.name !== 'AbortError') console.error(err);
    });
  
  return () => controller.abort();
}, []);
```

### Tarea 3: Event listeners
Agrega y remueve listeners:
```jsx
useEffect(() => {
  const handleResize = () => setWidth(window.innerWidth);
  window.addEventListener('resize', handleResize);
  return () => window.removeEventListener('resize', handleResize);
}, []);
```

## Ejercicios Adicionales
- Practica con websockets
- Experimenta con subscripciones
