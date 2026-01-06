# Día 7: Práctica Integradora

En este día realizarás ejercicios que integran todos los conceptos de la semana.

## Contenido
- Repaso de JWT
- Repaso de registro y login
- Repaso de autorización
- Proyecto integrador

## Proyecto del Día

### Proyecto: API Segura con Autenticación Completa

Crea una API con sistema de autenticación completo:

1. **Endpoints de autenticación:**
   - POST /api/auth/register - Registro
   - POST /api/auth/login - Login
   - GET /api/auth/profile - Perfil (protegido)
   - POST /api/auth/refresh - Refresh token

2. **Sistema de usuarios:**
   - Roles: user, moderator, admin
   - Modelo con password hasheado
   - Validaciones robustas

3. **Protección de rutas:**
   - Rutas públicas vs protegidas
   - Rutas por rol
   - Verificación de propiedad

4. **API de recursos (ej: posts):**
   - CRUD de posts
   - Solo autenticados pueden crear
   - Solo autor o admin puede editar/eliminar
   - Todos pueden leer

5. **Seguridad:**
   - Contraseñas hasheadas
   - Tokens con expiración
   - Manejo de errores seguro

## Tareas Adicionales

### Tarea 1: Refresh tokens
Implementa sistema de refresh tokens.

### Tarea 2: Logout
Implementa invalidación de tokens.

## Ejercicios de Repaso
- Revisa los conceptos que te costaron más durante la semana
- Practica los ejercicios que no completaste de días anteriores
