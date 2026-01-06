# Día 2: Setup de Jest

En este día configurarás Jest en tu proyecto.

## Contenido
- Instalación de Jest
- Configuración básica
- Primer test
- Scripts npm

## Tareas

### Tarea 1: Instalar Jest
Configura Jest:
```bash
npm install --save-dev jest
```
En package.json:
```json
"scripts": {
  "test": "jest"
}
```

### Tarea 2: Primer test
Crea sum.test.js:
```javascript
const sum = (a, b) => a + b;

test('suma 1 + 2 es igual a 3', () => {
  expect(sum(1, 2)).toBe(3);
});
```
Ejecuta: npm test

### Tarea 3: Configuración
Crea jest.config.js:
```javascript
module.exports = {
  testEnvironment: 'node',
  verbose: true,
};
```

## Ejercicios Adicionales
- Experimenta con diferentes matchers
- Practica con describe para agrupar tests
