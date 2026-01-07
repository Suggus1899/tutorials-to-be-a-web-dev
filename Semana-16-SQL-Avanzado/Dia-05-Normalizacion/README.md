# Día 5: Normalización

En este día aprenderás sobre normalización de bases de datos.

## Contenido
- Qué es la normalización
- Primera Forma Normal (1NF)
- Segunda Forma Normal (2NF)
- Tercera Forma Normal (3NF)

## Tareas

### Tarea 1: Identificar problemas
Analiza esta tabla y encuentra problemas:
```
pedidos (id, cliente_nombre, cliente_email, producto, cantidad)
```
- Datos duplicados
- Anomalías de inserción/actualización/eliminación

### Tarea 2: Normalizar a 1NF
Asegura que:
- Cada columna tiene valores atómicos
- No hay grupos repetitivos
- Cada fila es única

### Tarea 3: Normalizar a 2NF y 3NF
Separa la tabla en:
- clientes (id, nombre, email)
- productos (id, nombre, precio)
- pedidos (id, cliente_id, producto_id, cantidad)

## Ejercicios Adicionales
- Practica normalizando tablas de ejemplos reales
- Investiga cuándo la desnormalización es útil
