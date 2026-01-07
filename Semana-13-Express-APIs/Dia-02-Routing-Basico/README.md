# Día 2: Routing Básico

En este día aprenderás sobre el sistema de routing de Express.

## Contenido
- Definir rutas
- Parámetros de ruta (:id)
- Query parameters (?key=value)
- Express Router

## Tareas

### Tarea 1: Parámetros de ruta
Crea rutas con parámetros:
- /users/:id → Obtener usuario por ID
- /products/:category/:id → Parámetros múltiples
- Accede a params con req.params

### Tarea 2: Query parameters
Practica con query strings:
- /search?q=texto → Búsqueda
- /products?category=x&page=1 → Filtros
- Accede con req.query

### Tarea 3: Express Router
Organiza rutas con Router:
- Crea un router para /api/users
- Crea un router para /api/products
- Monta los routers en la app principal

## Ejercicios Adicionales
- Experimenta con req.path y req.url
- Practica con rutas que acepten parámetros opcionales
