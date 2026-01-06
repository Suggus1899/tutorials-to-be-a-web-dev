# Día 4: Tipos de Datos y Constraints

En este día aprenderás sobre tipos de datos y restricciones.

## Contenido
- Tipos de datos en SQLite
- NOT NULL, UNIQUE
- DEFAULT values
- CHECK constraints

## Tareas

### Tarea 1: Tipos de datos
Crea tablas usando diferentes tipos:
- INTEGER para números enteros
- REAL para decimales
- TEXT para strings
- BLOB para datos binarios

### Tarea 2: Constraints
Practica con restricciones:
- NOT NULL para campos obligatorios
- UNIQUE para valores únicos
- DEFAULT para valores por defecto
- CHECK para validaciones

### Tarea 3: Tabla completa
Crea una tabla de empleados con:
```sql
CREATE TABLE empleados (
  id INTEGER PRIMARY KEY AUTOINCREMENT,
  nombre TEXT NOT NULL,
  email TEXT UNIQUE NOT NULL,
  salario REAL DEFAULT 0,
  activo INTEGER DEFAULT 1,
  created_at TEXT DEFAULT CURRENT_TIMESTAMP
);
```

## Ejercicios Adicionales
- Investiga diferencias con otros RDBMS
- Practica con AUTOINCREMENT
