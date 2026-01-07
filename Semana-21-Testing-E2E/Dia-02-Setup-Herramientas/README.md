# Día 2: Setup de Herramientas E2E

En este día configurarás una herramienta de testing E2E.

## Contenido
- Instalación de Cypress/Playwright
- Configuración inicial
- Estructura de proyecto
- Primer test

## Tareas

### Tarea 1: Instalar Cypress
Configura Cypress:
```bash
npm install --save-dev cypress
npx cypress open
```
O Playwright:
```bash
npm install --save-dev @playwright/test
npx playwright install
```

### Tarea 2: Primer test
Crea un test básico:
```javascript
// Cypress
describe('Mi primera prueba', () => {
  it('visita la página principal', () => {
    cy.visit('http://localhost:3000');
    cy.contains('Bienvenido');
  });
});
```

### Tarea 3: Explorar la UI
Familiarízate con:
- Test runner interactivo
- Selectores de elementos
- Time travel debugging

## Ejercicios Adicionales
- Configura scripts en package.json
- Practica con headless mode
