# Día 2: useState Avanzado

En este día aprenderás patrones avanzados de useState.

## Contenido
- Estado con objetos
- Estado con arrays
- Actualización funcional
- Inmutabilidad

## Tareas

### Tarea 1: Estado con objetos
Actualiza objetos inmutablemente:
```jsx
const [user, setUser] = useState({ name: '', email: '' });

// Actualizar una propiedad
setUser({ ...user, name: 'Juan' });
```

### Tarea 2: Estado con arrays
Manipula arrays:
```jsx
const [items, setItems] = useState([]);

// Agregar
setItems([...items, newItem]);

// Eliminar
setItems(items.filter(item => item.id !== id));

// Actualizar
setItems(items.map(item => item.id === id ? {...item, done: true} : item));
```

### Tarea 3: Actualización funcional
Usa cuando dependes del estado anterior:
```jsx
setCount(prevCount => prevCount + 1);
```

## Ejercicios Adicionales
- Crea una lista de tareas
- Practica con formularios complejos
