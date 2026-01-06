# Día 6: Redux Avanzado

En este día aprenderás patrones avanzados de Redux.

## Contenido
- Selectors con createSelector
- Redux DevTools
- RTK Query (intro)
- Mejores prácticas

## Tareas

### Tarea 1: Selectors
Crea selectors memoizados:
```jsx
import { createSelector } from '@reduxjs/toolkit';

const selectTodos = state => state.todos;
const selectFilter = state => state.filter;

const selectVisibleTodos = createSelector(
  [selectTodos, selectFilter],
  (todos, filter) => todos.filter(todo => todo.status === filter)
);
```

### Tarea 2: Redux DevTools
Usa Redux DevTools:
- Inspecciona el estado
- Time travel debugging
- Exportar/importar estado

### Tarea 3: Organización
Organiza tu código Redux:
```
store/
  index.js
  slices/
    userSlice.js
    productSlice.js
  selectors/
    userSelectors.js
```

## Ejercicios Adicionales
- Explora RTK Query para data fetching
- Practica con persistencia de estado
