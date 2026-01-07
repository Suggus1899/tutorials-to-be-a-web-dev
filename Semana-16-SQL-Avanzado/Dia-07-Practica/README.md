# Día 7: Práctica Integradora

En este día realizarás ejercicios que integran todos los conceptos de la semana.

## Contenido
- Repaso de JOINs
- Repaso de relaciones y Foreign Keys
- Repaso de normalización
- Proyecto integrador

## Proyecto del Día

### Proyecto: Base de Datos para Sistema de E-commerce

Diseña e implementa una base de datos completa:

1. **Tablas a crear:**
   - usuarios (id, nombre, email, password_hash)
   - categorias (id, nombre, parent_id para subcategorías)
   - productos (id, nombre, descripcion, precio, stock, categoria_id)
   - pedidos (id, usuario_id, fecha, total, estado)
   - detalles_pedido (id, pedido_id, producto_id, cantidad, precio_unitario)

2. **Relaciones:**
   - Usuario → Pedidos (1:N)
   - Pedido → Detalles (1:N)
   - Producto → Detalles (1:N)
   - Categoría → Productos (1:N)
   - Categoría → Subcategorías (self-reference)

3. **Consultas a implementar:**
   - Listar pedidos de un usuario con detalles
   - Productos por categoría con JOIN
   - Total gastado por usuario
   - Productos más vendidos

4. **Datos de prueba:**
   - Al menos 10 usuarios
   - 5 categorías con subcategorías
   - 20 productos
   - Varios pedidos con detalles

## Tareas Adicionales

### Tarea 1: Funciones de agregación
Usa COUNT, SUM, AVG para reportes.

### Tarea 2: Vistas
Crea vistas para consultas frecuentes.

## Ejercicios de Repaso
- Revisa los conceptos que te costaron más durante la semana
- Practica los ejercicios que no completaste de días anteriores
