# Día 2: Rutas Básicas

En este día aprenderás a definir rutas.

## Contenido
- Routes y Route
- Element prop
- Rutas anidadas
- Outlet

## Tareas

### Tarea 1: Definir rutas
Crea rutas básicas:
```jsx
import { Routes, Route } from 'react-router-dom';

function App() {
  return (
    <Routes>
      <Route path="/" element={<Home />} />
      <Route path="/about" element={<About />} />
      <Route path="/contact" element={<Contact />} />
    </Routes>
  );
}
```

### Tarea 2: Página 404
Agrega ruta catch-all:
```jsx
<Route path="*" element={<NotFound />} />
```

### Tarea 3: Rutas anidadas
Usa Outlet para layouts:
```jsx
<Route path="/dashboard" element={<DashboardLayout />}>
  <Route index element={<DashboardHome />} />
  <Route path="settings" element={<Settings />} />
</Route>
```

## Ejercicios Adicionales
- Crea múltiples layouts
- Practica con index routes
