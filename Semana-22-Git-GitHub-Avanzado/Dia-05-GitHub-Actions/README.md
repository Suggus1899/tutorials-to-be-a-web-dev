# Día 5: GitHub Actions

En este día aprenderás a crear workflows automatizados.

## Contenido
- Qué son GitHub Actions
- Anatomía de un workflow
- Triggers y eventos
- Jobs y steps

## Tareas

### Tarea 1: Primer workflow
Crea .github/workflows/ci.yml:
```yaml
name: CI
on: [push, pull_request]
jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v3
      - uses: actions/setup-node@v3
        with:
          node-version: 18
      - run: npm ci
      - run: npm test
```

### Tarea 2: Diferentes triggers
Practica con eventos:
- push a ramas específicas
- pull_request
- schedule (cron)
- workflow_dispatch (manual)

### Tarea 3: Múltiples jobs
Crea workflow con varios jobs:
- lint
- test
- build
- Dependencias entre jobs

## Ejercicios Adicionales
- Usa secrets para variables sensibles
- Practica con matrix builds
