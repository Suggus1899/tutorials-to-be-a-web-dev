# Día 6: Resolución de Problemas

En este día aprenderás estrategias para encontrar y resolver errores.

## Contenido
- Herramientas de debugging del navegador
- Breakpoints y step-by-step
- Estrategias para encontrar errores
- Errores comunes en JavaScript

## Tareas

### Tarea 1: Usar DevTools
Abre las herramientas de desarrollador de tu navegador y practica:
- Colocar breakpoints
- Ejecutar código paso a paso
- Inspeccionar variables

### Tarea 2: Depurar código con errores
Encuentra y corrige los errores en el siguiente código:
```javascript
function verificarEdad(edad) {
    if (edad >= 18) {
        return "Mayor de edad"
    } else if (edad >= 13) {
        return "Adolescente"
    } else if (edad >= 0) {
        return "Niño"
    }
}

console.log(verificarEdad(-5)); // ¿Qué retorna? ¿Es correcto?
```

### Tarea 3: Documentar proceso de debugging
Escribe un pequeño reporte describiendo cómo encontrarías un error en un programa.

## Ejercicios Adicionales
- Practica con el debugger de tu editor de código
- Investiga sobre el uso de try/catch para manejo de errores
