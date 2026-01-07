# Día 3: Relaciones

En este día aprenderás sobre tipos de relaciones entre tablas.

## Contenido
- One-to-One
- One-to-Many
- Many-to-Many
- Tablas intermedias

## Tareas

### Tarea 1: Relación One-to-Many
Crea y practica:
- Categoría → Productos (una categoría, muchos productos)
- Usuario → Posts
- Cliente → Pedidos

### Tarea 2: Relación Many-to-Many
Crea tablas con relación muchos a muchos:
```sql
CREATE TABLE estudiantes (id INTEGER PRIMARY KEY, nombre TEXT);
CREATE TABLE cursos (id INTEGER PRIMARY KEY, nombre TEXT);
CREATE TABLE matriculas (
  estudiante_id INTEGER,
  curso_id INTEGER,
  PRIMARY KEY (estudiante_id, curso_id)
);
```

### Tarea 3: Consultas con Many-to-Many
Practica:
- Obtener cursos de un estudiante
- Obtener estudiantes de un curso
- JOIN con tabla intermedia

## Ejercicios Adicionales
- Diseña relaciones para una red social
- Practica con datos más complejos
