# Día 6: Autorización

En este día aprenderás a implementar autorización basada en roles.

## Contenido
- Diferencia autenticación vs autorización
- Roles y permisos
- Middleware de autorización
- Mejores prácticas

## Tareas

### Tarea 1: Agregar roles
Modifica el modelo de usuario:
- Agrega campo role (user, admin)
- Incluye role en el token JWT

### Tarea 2: Middleware de roles
Crea middleware de autorización:
```javascript
function authorize(...roles) {
  return (req, res, next) => {
    if (!roles.includes(req.user.role)) {
      return res.status(403).json({ error: 'No autorizado' });
    }
    next();
  };
}

// Uso
router.delete('/users/:id', authMiddleware, authorize('admin'), deleteUser);
```

### Tarea 3: Permisos granulares
Implementa:
- Verificar propiedad de recursos
- Solo el autor puede editar su post
- Admin puede editar cualquier post

## Ejercicios Adicionales
- Implementa sistema de permisos más complejo
- Practica con RBAC (Role-Based Access Control)
