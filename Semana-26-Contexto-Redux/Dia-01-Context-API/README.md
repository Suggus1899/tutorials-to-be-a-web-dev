# Día 1: Context API

En este día aprenderás los fundamentos de Context API.

## Contenido
- Por qué Context
- Crear contextos
- Provider pattern
- Cuándo usar Context

## Tareas

### Tarea 1: Crear un Context
Crea ThemeContext:
```jsx
import { createContext } from 'react';

export const ThemeContext = createContext('light');
```

### Tarea 2: Provider
Proporciona el contexto:
```jsx
import { ThemeContext } from './ThemeContext';

function App() {
  const [theme, setTheme] = useState('light');
  
  return (
    <ThemeContext.Provider value={{ theme, setTheme }}>
      <MainContent />
    </ThemeContext.Provider>
  );
}
```

### Tarea 3: Consumir contexto
Usa useContext:
```jsx
import { useContext } from 'react';
import { ThemeContext } from './ThemeContext';

function Button() {
  const { theme, setTheme } = useContext(ThemeContext);
  return <button onClick={() => setTheme('dark')}>{theme}</button>;
}
```

## Ejercicios Adicionales
- Crea contexto de usuario
- Practica con múltiples contextos
