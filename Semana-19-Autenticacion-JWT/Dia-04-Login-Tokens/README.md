# Día 4: Login y Generación de Tokens

En este día implementarás el login y generación de JWT.

## Contenido
- Endpoint de login
- Verificación de credenciales
- Generación de JWT
- Configuración de expiración

## Tareas

### Tarea 1: Instalar jsonwebtoken
Configura:
```bash
npm install jsonwebtoken
```

### Tarea 2: Endpoint de login
Crea POST /api/auth/login:
```javascript
const jwt = require('jsonwebtoken');

// Verificar credenciales
const user = await findUserByEmail(email);
const validPassword = await bcrypt.compare(password, user.password);

// Generar token
const token = jwt.sign(
  { userId: user.id, email: user.email },
  process.env.JWT_SECRET,
  { expiresIn: '24h' }
);
```

### Tarea 3: Configuración segura
Implementa:
- JWT_SECRET en variables de entorno
- Expiración apropiada
- Payload mínimo necesario

## Ejercicios Adicionales
- Implementa refresh tokens
- Practica con diferentes tiempos de expiración
