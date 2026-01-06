# Día 5: Middleware de Autenticación

En este día crearás un middleware para proteger rutas.

## Contenido
- Middleware de verificación
- Header Authorization
- Bearer token
- Manejo de errores de auth

## Tareas

### Tarea 1: Crear middleware
Crea authMiddleware.js:
```javascript
const jwt = require('jsonwebtoken');

function authMiddleware(req, res, next) {
  const authHeader = req.headers.authorization;
  if (!authHeader?.startsWith('Bearer ')) {
    return res.status(401).json({ error: 'Token no proporcionado' });
  }
  
  const token = authHeader.split(' ')[1];
  try {
    const decoded = jwt.verify(token, process.env.JWT_SECRET);
    req.user = decoded;
    next();
  } catch (error) {
    res.status(401).json({ error: 'Token inválido' });
  }
}
```

### Tarea 2: Proteger rutas
Aplica el middleware:
```javascript
router.get('/profile', authMiddleware, getProfile);
```

### Tarea 3: Acceder al usuario
Usa req.user en controladores:
- Obtener perfil del usuario autenticado
- Crear recursos asociados al usuario

## Ejercicios Adicionales
- Maneja tokens expirados con mensaje específico
- Implementa logout (blacklist de tokens)
