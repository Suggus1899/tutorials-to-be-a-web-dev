# Día 2: Conexión a Base de Datos

En este día aprenderás a gestionar conexiones de forma profesional.

## Contenido
- Patrones de conexión
- Manejo de errores
- Promisificar sqlite3
- Singleton pattern

## Tareas

### Tarea 1: Promisificar operaciones
Convierte callbacks a promesas:
```javascript
function dbAll(sql, params = []) {
  return new Promise((resolve, reject) => {
    db.all(sql, params, (err, rows) => {
      if (err) reject(err);
      else resolve(rows);
    });
  });
}
```

### Tarea 2: Módulo de conexión
Crea un módulo database.js:
- Exporta la conexión
- Maneja apertura/cierre
- Implementa singleton

### Tarea 3: Async/await con la BD
Practica:
- Usa async/await para operaciones
- Maneja errores con try/catch
- Crea funciones helper reutilizables

## Ejercicios Adicionales
- Investiga connection pooling (para otras BDs)
- Practica con transacciones
