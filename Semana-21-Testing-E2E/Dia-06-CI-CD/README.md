# Día 6: CI/CD Integration

En este día aprenderás a integrar E2E tests en CI/CD.

## Contenido
- Tests en CI/CD
- Headless mode
- Reportes
- Mejores prácticas

## Tareas

### Tarea 1: Headless mode
Ejecuta tests sin UI:
```bash
npx cypress run --headless
npx playwright test
```

### Tarea 2: GitHub Actions
Configura CI:
```yaml
- name: Run E2E tests
  run: |
    npm start &
    npx wait-on http://localhost:3000
    npx cypress run
```

### Tarea 3: Reportes
Configura reportes:
- Screenshots de fallos
- Videos de tests
- Reportes HTML

## Ejercicios Adicionales
- Configura tests paralelos
- Practica con retries para tests flaky
