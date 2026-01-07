# Día 6: Coverage y Mejores Prácticas

En este día aprenderás sobre coverage y mejores prácticas.

## Contenido
- Code coverage
- Reportes de coverage
- Mejores prácticas de testing
- Cuánto coverage es suficiente

## Tareas

### Tarea 1: Generar coverage
Ejecuta con coverage:
```bash
npx jest --coverage
```
Revisa el reporte en coverage/lcov-report/index.html

### Tarea 2: Configurar umbrales
En jest.config.js:
```javascript
coverageThreshold: {
  global: {
    branches: 80,
    functions: 80,
    lines: 80,
    statements: 80
  }
}
```

### Tarea 3: Mejores prácticas
Aplica:
- Tests independientes
- Nombres descriptivos
- AAA pattern (Arrange, Act, Assert)
- Evitar tests frágiles

## Ejercicios Adicionales
- Integra coverage con CI/CD
- Practica mejorando coverage de código existente
