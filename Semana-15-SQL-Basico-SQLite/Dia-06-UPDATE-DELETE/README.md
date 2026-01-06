# Día 6: UPDATE y DELETE

En este día aprenderás a actualizar y eliminar datos.

## Contenido
- UPDATE para modificar datos
- DELETE para eliminar registros
- Importancia del WHERE
- Transacciones básicas

## Tareas

### Tarea 1: UPDATE básico
Practica actualizando:
```sql
UPDATE usuarios SET nombre = 'Juan Carlos' WHERE id = 1;
```
- Actualiza un campo
- Actualiza múltiples campos
- Actualiza múltiples registros

### Tarea 2: DELETE básico
Practica eliminando:
```sql
DELETE FROM usuarios WHERE id = 1;
```
- Elimina un registro específico
- Elimina múltiples registros
- ¡Cuidado! DELETE sin WHERE elimina todo

### Tarea 3: Prácticas seguras
Implementa:
- Siempre usa WHERE
- Verifica con SELECT antes de UPDATE/DELETE
- Practica con transacciones (BEGIN, COMMIT, ROLLBACK)

## Ejercicios Adicionales
- Implementa soft delete (columna deleted)
- Practica con TRUNCATE vs DELETE
