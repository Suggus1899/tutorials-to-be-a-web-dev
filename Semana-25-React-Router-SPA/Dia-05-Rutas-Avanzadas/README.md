# Día 5: Rutas Avanzadas

En este día aprenderás patrones avanzados de routing.

## Contenido
- Lazy loading
- Loaders y actions
- Error boundaries
- Redirects

## Tareas

### Tarea 1: Lazy loading
Carga componentes bajo demanda:
```jsx
import { lazy, Suspense } from 'react';

const Dashboard = lazy(() => import('./Dashboard'));

<Route 
  path="/dashboard" 
  element={
    <Suspense fallback={<Loading />}>
      <Dashboard />
    </Suspense>
  } 
/>
```

### Tarea 2: Redirect
Redirige rutas:
```jsx
import { Navigate } from 'react-router-dom';

<Route path="/old-path" element={<Navigate to="/new-path" replace />} />
```

### Tarea 3: Error boundaries
Maneja errores de ruta:
```jsx
<Route 
  path="/users" 
  element={<Users />}
  errorElement={<ErrorPage />}
/>
```

## Ejercicios Adicionales
- Implementa loading indicators
- Practica con data loading
