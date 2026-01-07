# Día 1: useState Básico

En este día aprenderás el hook useState.

## Contenido
- Qué es el estado
- useState hook
- Actualizar estado
- Re-renders

## Tareas

### Tarea 1: Primer useState
Crea un contador:
```jsx
import { useState } from 'react';

function Counter() {
  const [count, setCount] = useState(0);
  
  return (
    <div>
      <p>Contador: {count}</p>
      <button onClick={() => setCount(count + 1)}>+1</button>
    </div>
  );
}
```

### Tarea 2: Estado con diferentes tipos
Practica con:
- Números (contador)
- Strings (input)
- Booleanos (toggle)

### Tarea 3: Múltiples estados
Usa varios useState:
```jsx
const [name, setName] = useState('');
const [age, setAge] = useState(0);
const [isActive, setIsActive] = useState(true);
```

## Ejercicios Adicionales
- Crea un toggle dark/light mode
- Practica con inputs controlados
