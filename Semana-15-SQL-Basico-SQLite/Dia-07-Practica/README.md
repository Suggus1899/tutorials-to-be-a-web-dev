# Día 7: Práctica Integradora

En este día realizarás ejercicios que integran todos los conceptos de la semana.

## Contenido
- Repaso de SQL básico
- Repaso de operaciones CRUD
- Repaso de constraints
- Proyecto integrador

## Proyecto del Día

### Proyecto: Base de Datos para Sistema de Inventario

Crea una base de datos completa para un sistema de inventario:

1. **Tablas a crear:**
   - productos (id, nombre, descripcion, precio, stock, categoria_id)
   - categorias (id, nombre, descripcion)
   - proveedores (id, nombre, contacto, telefono)
   - movimientos (id, producto_id, tipo, cantidad, fecha)

2. **Datos de prueba:**
   - Inserta al menos 5 categorías
   - Inserta al menos 10 productos
   - Inserta algunos movimientos de inventario

3. **Consultas a implementar:**
   - Listar todos los productos
   - Buscar productos por nombre
   - Productos con stock bajo (< 10)
   - Productos ordenados por precio
   - Productos filtrados por categoría

4. **Operaciones CRUD:**
   - Agregar nuevo producto
   - Actualizar precio de producto
   - Actualizar stock
   - Eliminar producto

## Tareas Adicionales

### Tarea 1: Reportes
Crea consultas de resumen (productos por categoría, valor total inventario).

### Tarea 2: Script SQL
Crea un archivo .sql con todo el schema y datos de prueba.

## Ejercicios de Repaso
- Revisa los conceptos que te costaron más durante la semana
- Practica los ejercicios que no completaste de días anteriores
