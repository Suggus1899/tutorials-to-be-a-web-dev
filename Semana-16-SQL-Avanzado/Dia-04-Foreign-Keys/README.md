# Día 4: Foreign Keys

En este día aprenderás sobre claves foráneas.

## Contenido
- Qué es una Foreign Key
- Definir Foreign Keys
- Integridad referencial
- ON DELETE / ON UPDATE

## Tareas

### Tarea 1: Definir Foreign Keys
Crea tablas con FK:
```sql
CREATE TABLE categorias (id INTEGER PRIMARY KEY, nombre TEXT);
CREATE TABLE productos (
  id INTEGER PRIMARY KEY,
  nombre TEXT,
  categoria_id INTEGER,
  FOREIGN KEY (categoria_id) REFERENCES categorias(id)
);
```

### Tarea 2: Habilitar Foreign Keys en SQLite
En SQLite, habilita FK:
```sql
PRAGMA foreign_keys = ON;
```
Prueba que funcione intentando insertar datos inválidos.

### Tarea 3: Acciones referenciales
Practica con ON DELETE:
- CASCADE: elimina productos al eliminar categoría
- SET NULL: pone NULL en productos
- RESTRICT: impide eliminar categoría con productos

## Ejercicios Adicionales
- Experimenta con ON UPDATE
- Diseña un schema con múltiples FKs
