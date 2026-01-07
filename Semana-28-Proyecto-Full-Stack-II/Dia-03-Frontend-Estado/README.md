# Día 3: Frontend - Estado

En este día implementarás el manejo de estado.

## Contenido
- Contexto de autenticación
- Estado global (Redux o Context)
- Servicios de API
- Hooks personalizados

## Tareas

### Tarea 1: Auth Context
Crea contexto de autenticación:
- Login/logout
- Guardar token
- Verificar autenticación
- Rutas protegidas

### Tarea 2: Servicios de API
Crea servicios con Axios:
```jsx
// api.js
const api = axios.create({ baseURL: 'http://localhost:3000/api' });

// Interceptor para agregar token
api.interceptors.request.use(config => {
  const token = localStorage.getItem('token');
  if (token) config.headers.Authorization = `Bearer ${token}`;
  return config;
});
```

### Tarea 3: Custom hooks
Crea hooks reutilizables:
- useAuth
- useFetch
- useForm

## Ejercicios Adicionales
- Implementa loading states
- Agrega manejo de errores global
