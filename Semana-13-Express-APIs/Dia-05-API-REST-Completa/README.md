# Día 5: API REST Completa

En este día crearás una API REST siguiendo convenciones.

## Contenido
- Convenciones REST
- Nombres de recursos
- Respuestas consistentes
- Documentación básica

## Tareas

### Tarea 1: API de recursos
Crea una API completa para un recurso (ej: tareas, productos):
- Todos los endpoints CRUD
- Estructura de respuesta consistente
- Manejo de errores uniforme

### Tarea 2: Respuestas consistentes
Implementa un formato de respuesta:
```javascript
{
  success: true,
  data: { ... },
  message: "Operación exitosa"
}
```
Para errores:
```javascript
{
  success: false,
  error: "Mensaje de error"
}
```

### Tarea 3: Paginación
Implementa paginación en endpoints GET:
- ?page=1&limit=10
- Retorna metadatos (total, páginas)

## Ejercicios Adicionales
- Implementa ordenamiento (?sort=name&order=asc)
- Documenta tu API con comentarios o un README
