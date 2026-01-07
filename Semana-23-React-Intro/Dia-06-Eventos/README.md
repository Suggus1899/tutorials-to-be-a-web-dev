# Día 6: Eventos

En este día aprenderás a manejar eventos en React.

## Contenido
- Eventos en JSX
- Event handlers
- Pasar datos a handlers
- Eventos comunes

## Tareas

### Tarea 1: Click events
Maneja clicks:
```jsx
function Button() {
  function handleClick() {
    alert('Clickeado!');
  }
  return <button onClick={handleClick}>Click me</button>;
}
```

### Tarea 2: Eventos de formulario
Maneja inputs:
```jsx
function handleChange(e) {
  console.log(e.target.value);
}
<input onChange={handleChange} />
```

### Tarea 3: Pasar parámetros
Pasa datos al handler:
```jsx
function handleDelete(id) {
  console.log('Eliminar:', id);
}

{items.map(item => (
  <button onClick={() => handleDelete(item.id)}>Eliminar</button>
))}
```

## Ejercicios Adicionales
- Practica con onSubmit
- Experimenta con onKeyDown
