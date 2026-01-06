# Día 3: Registro de Usuarios

En este día implementarás el registro de usuarios.

## Contenido
- Endpoint de registro
- Validación de datos
- Hash de contraseña
- Respuestas apropiadas

## Tareas

### Tarea 1: Endpoint de registro
Crea POST /api/auth/register:
- Recibe username, email, password
- Valida datos (email válido, password mínimo)
- Verifica que email no exista

### Tarea 2: Guardar usuario
Implementa:
- Hash de la contraseña
- Guardar en base de datos
- Retornar usuario sin password

### Tarea 3: Validaciones
Implementa validaciones:
- Email formato válido
- Password mínimo 8 caracteres
- Username alfanumérico
- Mensajes de error claros

## Ejercicios Adicionales
- Agrega confirmación de email (simulada)
- Implementa requisitos de password más estrictos
