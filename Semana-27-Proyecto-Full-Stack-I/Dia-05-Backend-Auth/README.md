# Día 5: Backend - Autenticación

En este día implementarás autenticación.

## Contenido
- Registro de usuarios
- Login con JWT
- Middleware de auth
- Autorización

## Tareas

### Tarea 1: Implementar registro
Crea POST /api/auth/register:
- Validación de datos
- Hash de password con bcrypt
- Guardar usuario
- Retornar token

### Tarea 2: Implementar login
Crea POST /api/auth/login:
- Verificar credenciales
- Generar JWT
- Retornar token y usuario

### Tarea 3: Middleware de auth
Crea middleware:
- Verificar token
- Adjuntar usuario a request
- Proteger rutas

## Ejercicios Adicionales
- Implementa refresh tokens
- Agrega validación con express-validator
