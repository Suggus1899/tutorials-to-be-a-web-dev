# Día 5: Listas

En este día aprenderás a renderizar listas.

## Contenido
- Renderizar arrays
- La prop key
- Filtrar elementos
- Mapear objetos

## Tareas

### Tarea 1: Renderizar lista
Usa map para listas:
```jsx
const frutas = ['Manzana', 'Banana', 'Naranja'];

return (
  <ul>
    {frutas.map((fruta, index) => (
      <li key={index}>{fruta}</li>
    ))}
  </ul>
);
```

### Tarea 2: Keys únicas
Usa IDs como keys:
```jsx
const users = [
  { id: 1, name: 'Juan' },
  { id: 2, name: 'María' }
];

{users.map(user => (
  <UserCard key={user.id} user={user} />
))}
```

### Tarea 3: Listas con objetos
Renderiza datos complejos:
- Lista de productos
- Lista de usuarios
- Lista de posts

## Ejercicios Adicionales
- Practica filtrando listas
- Experimenta con listas anidadas
