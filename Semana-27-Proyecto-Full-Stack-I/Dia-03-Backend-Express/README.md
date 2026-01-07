# Día 3: Backend con Express

En este día configurarás el backend.

## Contenido
- Setup del proyecto
- Estructura de carpetas
- Configurar Express
- Rutas básicas

## Tareas

### Tarea 1: Setup del proyecto
Inicializa el backend:
```bash
mkdir backend && cd backend
npm init -y
npm install express cors helmet morgan dotenv
npm install -D nodemon
```

### Tarea 2: Estructura de carpetas
Crea la estructura:
```
backend/
  src/
    config/
    controllers/
    middlewares/
    routes/
    services/
    app.js
    server.js
```

### Tarea 3: Express básico
Configura Express:
- Middlewares globales
- Rutas principales
- Manejo de errores
- Health check endpoint

## Ejercicios Adicionales
- Configura ESLint y Prettier
- Agrega scripts de desarrollo
