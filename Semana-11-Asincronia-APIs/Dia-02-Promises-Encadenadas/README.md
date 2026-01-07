# Día 2: Promises Encadenadas

En este día aprenderás a encadenar promesas y manejar múltiples operaciones asíncronas.

## Contenido
- Encadenar promesas con then()
- Promise.all()
- Promise.race()
- Promise.allSettled()

## Tareas

### Tarea 1: Encadenar promesas
Crea una secuencia donde:
- La primera promesa obtiene un ID de usuario
- La segunda usa ese ID para obtener datos del usuario
- La tercera procesa los datos

### Tarea 2: Promise.all
Practica:
- Ejecutar múltiples promesas en paralelo
- Esperar a que todas se resuelvan
- Manejar el caso donde una falla

### Tarea 3: Promise.race y Promise.allSettled
Practica:
- Obtener el resultado de la promesa más rápida
- Usar allSettled para obtener todos los resultados
- Implementar un timeout con Promise.race

## Ejercicios Adicionales
- Implementa Promise.any (primera que se resuelva exitosamente)
- Practica con Promise.allSettled para manejar errores parciales
