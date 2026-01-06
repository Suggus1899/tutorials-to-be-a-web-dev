# Día 3: Introducción a Middlewares

En este día aprenderás qué son los middlewares y cómo usarlos.

## Contenido
- Qué es un middleware
- El flujo de request/response
- next() function
- Middlewares de Express

## Tareas

### Tarea 1: Entender middlewares
Crea un middleware simple:
- Que imprima la fecha y hora de cada request
- Que imprima el método y la URL
- Usa next() para continuar

### Tarea 2: Middlewares de terceros
Instala y configura:
- cors para Cross-Origin
- morgan para logging
- helmet para seguridad

### Tarea 3: Orden de middlewares
Experimenta con:
- El orden de app.use()
- Middlewares globales vs por ruta
- Middlewares que terminan la respuesta

## Ejercicios Adicionales
- Investiga cómo funciona express.json()
- Practica con express.static() para archivos
