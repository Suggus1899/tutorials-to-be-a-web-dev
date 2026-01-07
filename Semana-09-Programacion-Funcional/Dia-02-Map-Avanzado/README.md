# Día 2: Map Avanzado

En este día aprenderás usos avanzados de map().

## Contenido
- Map con objetos complejos
- Transformaciones anidadas
- Encadenar map con otros métodos
- Casos de uso reales

## Tareas

### Tarea 1: Transformar estructura de datos
Dado un array de productos:
```javascript
const productos = [
  { nombre: "Laptop", precio: 1000, cantidad: 5 },
  { nombre: "Mouse", precio: 25, cantidad: 10 }
];
```
Transforma a:
- Array con precios con IVA
- Array con valor total (precio * cantidad)
- Nuevo formato { item: nombre, total: precio * cantidad }

### Tarea 2: Map anidado
Trabaja con arrays de arrays:
- Transforma una matriz de números
- Modifica objetos con arrays internos

### Tarea 3: Encadenar métodos
Combina map con otros métodos:
- map().join() para crear strings
- map().map() para transformaciones dobles

## Ejercicios Adicionales
- Implementa flatMap para aplanar y transformar
- Practica transformando datos de una API ficticia
