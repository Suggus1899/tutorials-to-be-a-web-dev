# Día 3: Selectores y Navegación

En este día aprenderás a seleccionar elementos y navegar.

## Contenido
- Selectores CSS
- Data attributes para testing
- Navegación entre páginas
- Esperas y timeouts

## Tareas

### Tarea 1: Selectores
Practica diferentes selectores:
```javascript
cy.get('button');              // por elemento
cy.get('.btn-primary');        // por clase
cy.get('#submit');             // por ID
cy.get('[data-testid="btn"]'); // por data attribute
```

### Tarea 2: Data-testid
Usa atributos específicos para testing:
```html
<button data-testid="submit-button">Enviar</button>
```
```javascript
cy.get('[data-testid="submit-button"]').click();
```

### Tarea 3: Navegación
Practica navegando:
```javascript
cy.visit('/');
cy.get('a[href="/about"]').click();
cy.url().should('include', '/about');
```

## Ejercicios Adicionales
- Practica con contains() para texto
- Experimenta con within() para scope
