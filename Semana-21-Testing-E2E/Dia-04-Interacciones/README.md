# Día 4: Interacciones

En este día aprenderás a simular interacciones de usuario.

## Contenido
- Clicks y doble clicks
- Escribir en inputs
- Formularios
- Uploads y selects

## Tareas

### Tarea 1: Clicks y typing
Practica interacciones:
```javascript
cy.get('button').click();
cy.get('input[name="email"]').type('test@email.com');
cy.get('input[name="password"]').type('password123');
cy.get('form').submit();
```

### Tarea 2: Formulario completo
Crea test para un formulario:
- Llena todos los campos
- Selecciona opciones de dropdown
- Marca checkboxes
- Envía el formulario
- Verifica resultado

### Tarea 3: Assertions
Practica verificaciones:
```javascript
cy.get('.message').should('be.visible');
cy.get('.message').should('contain', 'Éxito');
cy.get('input').should('have.value', 'test');
cy.url().should('include', '/dashboard');
```

## Ejercicios Adicionales
- Practica con hover y focus
- Experimenta con drag and drop
