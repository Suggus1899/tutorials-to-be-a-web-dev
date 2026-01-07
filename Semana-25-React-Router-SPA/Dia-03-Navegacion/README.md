# Día 3: Navegación

En este día aprenderás a navegar entre rutas.

## Contenido
- Link component
- NavLink para navegación activa
- useNavigate hook
- Navegación programática

## Tareas

### Tarea 1: Usar Link
Crea navegación:
```jsx
import { Link } from 'react-router-dom';

function Navbar() {
  return (
    <nav>
      <Link to="/">Home</Link>
      <Link to="/about">About</Link>
    </nav>
  );
}
```

### Tarea 2: NavLink activo
Estilos para ruta activa:
```jsx
import { NavLink } from 'react-router-dom';

<NavLink 
  to="/about" 
  className={({ isActive }) => isActive ? 'active' : ''}
>
  About
</NavLink>
```

### Tarea 3: Navegación programática
Usa useNavigate:
```jsx
import { useNavigate } from 'react-router-dom';

function Login() {
  const navigate = useNavigate();
  
  function handleLogin() {
    // login logic
    navigate('/dashboard');
  }
}
```

## Ejercicios Adicionales
- Practica con navigate(-1) para ir atrás
- Experimenta con replace: true
