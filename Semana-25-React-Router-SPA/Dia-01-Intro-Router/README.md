# Día 1: Introducción a React Router

En este día aprenderás los fundamentos de React Router.

## Contenido
- Qué es React Router
- SPA (Single Page Application)
- Instalación
- BrowserRouter

## Tareas

### Tarea 1: Instalar React Router
Configura React Router:
```bash
npm install react-router-dom
```

### Tarea 2: Configurar BrowserRouter
Envuelve tu app:
```jsx
import { BrowserRouter } from 'react-router-dom';

function App() {
  return (
    <BrowserRouter>
      <AppContent />
    </BrowserRouter>
  );
}
```

### Tarea 3: Entender SPA
Analiza:
- Diferencia con páginas tradicionales
- Navegación sin recargar
- Historial del navegador

## Ejercicios Adicionales
- Investiga HashRouter vs BrowserRouter
- Explora la documentación de React Router
