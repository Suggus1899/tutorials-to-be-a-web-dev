# Día 6: CI/CD Completo

En este día implementarás un pipeline CI/CD completo.

## Contenido
- Continuous Integration
- Continuous Deployment
- Environments
- Deploy automático

## Tareas

### Tarea 1: Pipeline CI
Crea pipeline completo:
```yaml
jobs:
  lint:
    runs-on: ubuntu-latest
    steps:
      - run: npm run lint
  test:
    runs-on: ubuntu-latest
    steps:
      - run: npm test
  build:
    needs: [lint, test]
    runs-on: ubuntu-latest
    steps:
      - run: npm run build
```

### Tarea 2: Deploy automático
Configura deploy:
- A Vercel/Netlify para frontend
- A Railway/Render para backend
- Usa secrets para tokens

### Tarea 3: Environments
Configura environments:
- Staging para PRs
- Production para main
- Protection rules

## Ejercicios Adicionales
- Implementa rollback automático
- Practica con deployment gates
