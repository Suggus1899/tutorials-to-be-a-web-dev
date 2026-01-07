# Día 5: Tests Avanzados

En este día aprenderás técnicas avanzadas de E2E testing.

## Contenido
- Fixtures y datos de prueba
- Mocking de API
- Page Object Model
- Custom commands

## Tareas

### Tarea 1: Fixtures
Usa datos externos:
```javascript
// cypress/fixtures/user.json
{ "email": "test@email.com", "password": "123456" }

// En el test
cy.fixture('user').then((user) => {
  cy.get('#email').type(user.email);
});
```

### Tarea 2: Interceptar API
Mockea respuestas de API:
```javascript
cy.intercept('GET', '/api/users', { fixture: 'users.json' });
cy.intercept('POST', '/api/login', { statusCode: 200, body: { token: 'fake' } });
```

### Tarea 3: Page Object Model
Organiza con Page Objects:
```javascript
class LoginPage {
  visit() { cy.visit('/login'); }
  fillEmail(email) { cy.get('#email').type(email); }
  submit() { cy.get('form').submit(); }
}
```

## Ejercicios Adicionales
- Crea custom commands reutilizables
- Practica con beforeEach para setup
