# Día 1: Driver SQLite para Node.js

En este día aprenderás a instalar y configurar el driver de SQLite.

## Contenido
- sqlite3 package para Node.js
- Instalación y configuración
- Diferencias con otras librerías
- Primeros pasos

## Tareas

### Tarea 1: Instalar sqlite3
Practica:
- Crea un nuevo proyecto Node.js
- Instala sqlite3 con npm install sqlite3
- Verifica la instalación importándolo

### Tarea 2: Crear conexión básica
Crea una conexión a la base de datos:
```javascript
const sqlite3 = require('sqlite3').verbose();
const db = new sqlite3.Database('./database.db');
```

### Tarea 3: Operaciones básicas
Practica con:
- db.run() para ejecutar sentencias
- db.get() para obtener un registro
- db.all() para obtener múltiples registros
- db.close() para cerrar conexión

## Ejercicios Adicionales
- Experimenta con better-sqlite3 (alternativa síncrona)
- Practica manejo de errores en conexión
