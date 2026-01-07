# Día 1: Controllers

En este día aprenderás a separar la lógica en controllers.

## Contenido
- Qué es un controller
- Separar lógica de rutas
- Funciones handler
- Estructura básica

## Tareas

### Tarea 1: Primer controller
Crea un controller de usuarios:
- Crea el archivo usersController.js
- Define funciones: getAll, getById, create, update, delete
- Cada función recibe req, res

### Tarea 2: Conectar controller con rutas
Refactoriza tus rutas:
- Importa las funciones del controller
- Reemplaza las funciones inline por el controller
- Mantén las rutas limpias y deleguen al controller

### Tarea 3: Múltiples controllers
Crea controllers adicionales:
- productsController.js
- ordersController.js
- Organiza en carpeta controllers/

## Ejercicios Adicionales
- Experimenta con controllers como clases
- Practica con controllers que compartan lógica común
