# Día 7: Práctica Integradora

En este día realizarás ejercicios que integran todos los conceptos de la semana.

## Contenido
- Repaso de conexión a BD
- Repaso de queries y seguridad
- Repaso de Repository Pattern
- Proyecto integrador

## Proyecto del Día

### Proyecto: API de Blog con Base de Datos

Crea una API completa de blog con persistencia en SQLite:

1. **Estructura de base de datos:**
   - users (id, username, email, password_hash, created_at)
   - posts (id, title, content, user_id, created_at, updated_at)
   - comments (id, content, post_id, user_id, created_at)

2. **Repositories a crear:**
   - userRepository
   - postRepository
   - commentRepository

3. **Endpoints API:**
   - CRUD completo para users, posts, comments
   - Obtener posts con autor
   - Obtener post con comentarios
   - Comentarios de un usuario

4. **Características:**
   - Prepared statements en todas las queries
   - Manejo de errores robusto
   - Transacciones donde corresponda
   - Scripts de migración y seed

## Tareas Adicionales

### Tarea 1: Búsqueda
Implementa búsqueda de posts por título o contenido.

### Tarea 2: Paginación
Agrega paginación a todos los endpoints de listado.

## Ejercicios de Repaso
- Revisa los conceptos que te costaron más durante la semana
- Practica los ejercicios que no completaste de días anteriores
