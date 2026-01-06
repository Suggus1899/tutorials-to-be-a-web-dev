# Día 4: CRUD - PUT y DELETE

En este día completarás las operaciones CRUD.

## Contenido
- PUT para actualizar recursos
- PATCH para actualizaciones parciales
- DELETE para eliminar recursos
- Status codes apropiados

## Tareas

### Tarea 1: Implementar PUT
Crea endpoint PUT:
- PUT /api/items/:id → Actualiza un item completo
- Verifica que el item exista (404 si no)
- Retorna el item actualizado

### Tarea 2: Implementar DELETE
Crea endpoint DELETE:
- DELETE /api/items/:id → Elimina un item
- Verifica que el item exista
- Retorna 204 No Content o el item eliminado

### Tarea 3: Implementar PATCH
Crea endpoint PATCH:
- PATCH /api/items/:id → Actualización parcial
- Solo modifica los campos enviados
- Mantiene los demás campos intactos

## Ejercicios Adicionales
- Implementa soft delete (marcar como eliminado)
- Practica con diferentes status codes
