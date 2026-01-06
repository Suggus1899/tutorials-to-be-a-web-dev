# Día 3: Crear Tablas

En este día aprenderás a crear tablas con CREATE TABLE.

## Contenido
- Sintaxis CREATE TABLE
- Definir columnas
- Primary Key
- Constraints básicos

## Tareas

### Tarea 1: Crear tabla básica
Crea una tabla de usuarios:
```sql
CREATE TABLE usuarios (
  id INTEGER PRIMARY KEY,
  nombre TEXT NOT NULL,
  email TEXT UNIQUE
);
```

### Tarea 2: Tabla con más columnas
Crea una tabla de productos:
- id, nombre, descripcion, precio, stock
- Usa tipos de datos apropiados
- Agrega constraints necesarios

### Tarea 3: Múltiples tablas
Crea un schema completo para un blog:
- Tabla autores
- Tabla posts
- Tabla comentarios

## Ejercicios Adicionales
- Practica con DROP TABLE
- Experimenta con ALTER TABLE
