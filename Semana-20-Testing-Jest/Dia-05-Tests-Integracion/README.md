# Día 5: Tests de Integración

En este día aprenderás a testear APIs con supertest.

## Contenido
- supertest para testing HTTP
- Testear endpoints Express
- Setup y teardown de DB
- Mejores prácticas

## Tareas

### Tarea 1: Instalar supertest
Configura:
```bash
npm install --save-dev supertest
```

### Tarea 2: Testear endpoints
Crea tests de API:
```javascript
const request = require('supertest');
const app = require('./app');

describe('GET /api/users', () => {
  it('should return all users', async () => {
    const res = await request(app).get('/api/users');
    expect(res.statusCode).toBe(200);
    expect(res.body).toHaveProperty('users');
  });
});
```

### Tarea 3: Test database
Configura BD de prueba:
- Usa BD separada para tests
- Limpia antes/después de tests
- Seed con datos de prueba

## Ejercicios Adicionales
- Testea endpoints protegidos con JWT
- Practica con diferentes status codes
