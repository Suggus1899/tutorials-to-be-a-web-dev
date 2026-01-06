# Día 5: Arquitectura de Capas

En este día aprenderás sobre la arquitectura de capas.

## Contenido
- Separación de responsabilidades
- Capa de presentación (routes)
- Capa de lógica de negocio (services)
- Capa de datos (repositories)

## Tareas

### Tarea 1: Crear capa de servicios
Separa la lógica:
- Crea una carpeta services/
- Mueve la lógica de negocio del controller al service
- El controller solo maneja request/response

### Tarea 2: Implementar servicios
Crea un userService con:
- getAllUsers()
- getUserById(id)
- createUser(data)
- Los métodos contienen la lógica real

### Tarea 3: Controller + Service
Conecta las capas:
- El controller llama al service
- El service retorna datos o lanza errores
- El controller formatea la respuesta

## Ejercicios Adicionales
- Agrega una capa de repositorio para datos
- Implementa inyección de dependencias básica
