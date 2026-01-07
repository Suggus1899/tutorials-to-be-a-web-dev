# Día 4: Middlewares Personalizados

En este día crearás tus propios middlewares.

## Contenido
- Crear middlewares personalizados
- Middlewares con parámetros
- Error handling middleware
- Middleware factories

## Tareas

### Tarea 1: Middleware de autenticación
Crea un middleware que:
- Verifique si existe un header Authorization
- Valide el token (simulado por ahora)
- Permita o rechace el acceso

### Tarea 2: Middleware de validación
Crea un middleware que:
- Valide el body de la request
- Retorne errores si faltan campos
- Sea configurable (reciba schema)

### Tarea 3: Error handling middleware
Implementa:
- Middleware de error global
- Diferentes tipos de errores
- Respuestas de error consistentes

## Ejercicios Adicionales
- Crea un middleware de rate limiting simple
- Implementa un middleware de caché básico
