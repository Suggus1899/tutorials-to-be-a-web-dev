# Día 6: Mejores Prácticas

En este día aprenderás mejores prácticas para trabajar con BD en Node.js.

## Contenido
- Manejo de errores de BD
- Transacciones
- Migraciones manuales
- Seeding de datos

## Tareas

### Tarea 1: Manejo de errores
Implementa:
- Errores específicos para BD
- Logging de queries fallidas
- Respuestas apropiadas al cliente

### Tarea 2: Transacciones
Implementa transacciones:
```javascript
db.serialize(() => {
  db.run("BEGIN TRANSACTION");
  // operaciones
  db.run("COMMIT");
  // o db.run("ROLLBACK") en caso de error
});
```

### Tarea 3: Scripts de migración
Crea scripts para:
- Inicializar la BD (crear tablas)
- Seeds con datos de prueba
- Reset de la BD para desarrollo

## Ejercicios Adicionales
- Investiga herramientas de migración
- Practica con backups de BD
