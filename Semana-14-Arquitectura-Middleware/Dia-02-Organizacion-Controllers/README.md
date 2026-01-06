# Día 2: Organización de Controllers

En este día aprenderás mejores prácticas para organizar controllers.

## Contenido
- Estructura de carpetas
- Naming conventions
- Manejo de errores en controllers
- Reutilización de código

## Tareas

### Tarea 1: Estructura de carpetas
Organiza tu proyecto:
```
src/
  controllers/
    userController.js
    productController.js
  routes/
    userRoutes.js
    productRoutes.js
```

### Tarea 2: Errores en controllers
Implementa:
- Try/catch en cada función
- Delegar errores al middleware de errores
- Códigos de estado apropiados

### Tarea 3: Helper functions
Crea funciones helper:
- Respuestas de éxito estandarizadas
- Respuestas de error estandarizadas
- Validaciones comunes

## Ejercicios Adicionales
- Implementa un base controller
- Practica con async handlers wrapper
