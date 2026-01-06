# Día 3: CRUD - GET y POST

En este día implementarás operaciones GET y POST.

## Contenido
- GET para obtener recursos
- POST para crear recursos
- express.json() middleware
- Parsear body de peticiones

## Tareas

### Tarea 1: Implementar GET
Crea endpoints GET:
- GET /api/items → Lista todos los items
- GET /api/items/:id → Obtiene un item específico
- Maneja el caso de item no encontrado (404)

### Tarea 2: Implementar POST
Crea endpoint POST:
- POST /api/items → Crea un nuevo item
- Usa express.json() para parsear el body
- Genera un ID único para cada item
- Retorna 201 Created

### Tarea 3: Validación básica
Implementa:
- Validación de campos requeridos
- Retorna 400 Bad Request si faltan datos
- Mensajes de error descriptivos

## Ejercicios Adicionales
- Guarda los datos en un array en memoria
- Implementa filtrado en GET con query parameters
