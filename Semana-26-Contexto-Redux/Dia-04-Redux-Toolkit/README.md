# Día 4: Redux Toolkit

En este día aprenderás Redux Toolkit, la forma moderna de usar Redux.

## Contenido
- Por qué Redux Toolkit
- createSlice
- configureStore
- useSelector y useDispatch

## Tareas

### Tarea 1: Instalar RTK
Configura Redux Toolkit:
```bash
npm install @reduxjs/toolkit react-redux
```

### Tarea 2: Crear un slice
Crea counterSlice:
```jsx
import { createSlice } from '@reduxjs/toolkit';

const counterSlice = createSlice({
  name: 'counter',
  initialState: { value: 0 },
  reducers: {
    increment: (state) => { state.value += 1 },
    decrement: (state) => { state.value -= 1 },
    incrementByAmount: (state, action) => { state.value += action.payload }
  }
});

export const { increment, decrement } = counterSlice.actions;
export default counterSlice.reducer;
```

### Tarea 3: Configurar store y usar
```jsx
// store.js
import { configureStore } from '@reduxjs/toolkit';
const store = configureStore({ reducer: { counter: counterReducer } });

// Component
const count = useSelector(state => state.counter.value);
const dispatch = useDispatch();
dispatch(increment());
```

## Ejercicios Adicionales
- Crea múltiples slices
- Practica con objetos más complejos
