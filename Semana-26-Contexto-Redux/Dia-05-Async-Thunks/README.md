# Día 5: Async Actions con Thunks

En este día aprenderás a manejar acciones asíncronas.

## Contenido
- createAsyncThunk
- Estados: pending, fulfilled, rejected
- extraReducers
- Manejo de errores

## Tareas

### Tarea 1: Crear async thunk
Crea acción asíncrona:
```jsx
import { createAsyncThunk } from '@reduxjs/toolkit';

export const fetchUsers = createAsyncThunk(
  'users/fetchUsers',
  async () => {
    const response = await fetch('/api/users');
    return response.json();
  }
);
```

### Tarea 2: Manejar estados
Usa extraReducers:
```jsx
extraReducers: (builder) => {
  builder
    .addCase(fetchUsers.pending, (state) => {
      state.loading = true;
    })
    .addCase(fetchUsers.fulfilled, (state, action) => {
      state.loading = false;
      state.users = action.payload;
    })
    .addCase(fetchUsers.rejected, (state, action) => {
      state.loading = false;
      state.error = action.error.message;
    });
}
```

### Tarea 3: Dispatch async
Usa en componentes:
```jsx
const dispatch = useDispatch();
const { users, loading, error } = useSelector(state => state.users);

useEffect(() => {
  dispatch(fetchUsers());
}, [dispatch]);
```

## Ejercicios Adicionales
- Implementa CRUD completo
- Practica con manejo de errores
