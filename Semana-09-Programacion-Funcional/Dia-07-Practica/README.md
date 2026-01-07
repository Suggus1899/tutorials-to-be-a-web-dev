# Día 7: Práctica Integradora

En este día realizarás ejercicios que integran todos los conceptos de la semana.

## Contenido
- Repaso de map
- Repaso de filter
- Repaso de reduce
- Proyecto integrador

## Proyecto del Día

### Proyecto: Procesador de Datos de Ventas

Crea un sistema que procese datos de ventas:

1. **Datos de entrada:**
   ```javascript
   const ventas = [
     { id: 1, producto: "Laptop", categoria: "Electronics", precio: 1000, cantidad: 2, fecha: "2024-01-15" },
     { id: 2, producto: "Mouse", categoria: "Electronics", precio: 25, cantidad: 5, fecha: "2024-01-15" },
     { id: 3, producto: "Camisa", categoria: "Ropa", precio: 30, cantidad: 3, fecha: "2024-01-16" },
     // más datos...
   ];
   ```

2. **Funciones a implementar:**
   - `calcularTotal(ventas)` - suma total de todas las ventas
   - `ventasPorCategoria(ventas)` - agrupa y suma por categoría
   - `ventasPorFecha(ventas)` - agrupa por fecha
   - `productosMasVendidos(ventas, n)` - top n productos
   - `resumenVentas(ventas)` - objeto con estadísticas completas

3. **Pipeline de datos:**
   - Encadena filter, map y reduce
   - Crea funciones reutilizables
   - Documenta cada función

## Tareas Adicionales

### Tarea 1: Agregar filtros
Permite filtrar por rango de fechas, categoría o precio mínimo.

### Tarea 2: Comparativas
Compara ventas entre diferentes períodos.

## Ejercicios de Repaso
- Revisa los conceptos que te costaron más durante la semana
- Practica los ejercicios que no completaste de días anteriores
