# Día 1: Introducción a JOINs

En este día aprenderás los fundamentos de JOIN en SQL.

## Contenido
- Qué es un JOIN
- Por qué necesitamos JOINs
- INNER JOIN básico
- Sintaxis y ejemplos

## Tareas

### Tarea 1: Preparar tablas relacionadas
Crea tablas para practicar:
```sql
CREATE TABLE autores (id INTEGER PRIMARY KEY, nombre TEXT);
CREATE TABLE libros (id INTEGER PRIMARY KEY, titulo TEXT, autor_id INTEGER);
```
Inserta datos de prueba.

### Tarea 2: Primer INNER JOIN
Practica uniendo tablas:
```sql
SELECT libros.titulo, autores.nombre
FROM libros
INNER JOIN autores ON libros.autor_id = autores.id;
```

### Tarea 3: JOINs con múltiples columnas
Practica:
- Seleccionar columnas de ambas tablas
- Usar alias para tablas (AS l, AS a)
- Agregar condiciones WHERE

## Ejercicios Adicionales
- Experimenta uniendo 3 tablas
- Practica con diferentes condiciones de JOIN
