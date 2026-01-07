# Día 7: Práctica Integradora

En este día realizarás ejercicios que integran todos los conceptos de la semana.

## Contenido
- Repaso de Prisma setup
- Repaso de modelos y relaciones
- Repaso de operaciones CRUD
- Proyecto integrador

## Proyecto del Día

### Proyecto: API de Red Social con Prisma

Crea una API de red social usando Prisma:

1. **Modelos a definir:**
   - User (id, email, username, bio, createdAt)
   - Post (id, content, authorId, createdAt)
   - Comment (id, content, postId, authorId, createdAt)
   - Like (id, postId, userId, createdAt)
   - Follow (id, followerId, followingId, createdAt)

2. **Relaciones:**
   - User → Posts (1:N)
   - User → Comments (1:N)
   - Post → Comments (1:N)
   - User ↔ User (followers/following, N:M)
   - User ↔ Post (likes, N:M)

3. **Endpoints API:**
   - CRUD de usuarios y posts
   - Agregar/eliminar comentarios
   - Like/unlike posts
   - Follow/unfollow usuarios
   - Feed de posts de usuarios seguidos

4. **Queries avanzadas:**
   - Posts con autor y conteo de likes
   - Usuario con seguidores y seguidos
   - Posts ordenados por popularidad

## Tareas Adicionales

### Tarea 1: Paginación
Implementa paginación cursor-based.

### Tarea 2: Búsqueda
Busca usuarios por username o posts por contenido.

## Ejercicios de Repaso
- Revisa los conceptos que te costaron más durante la semana
- Practica los ejercicios que no completaste de días anteriores
