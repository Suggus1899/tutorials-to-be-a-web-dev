# Día 5: Migrations y CRUD

En este día aprenderás a crear migraciones y operaciones CRUD.

## Contenido
- Crear migraciones
- Prisma Client
- Operaciones CRUD
- Type safety

## Tareas

### Tarea 1: Crear migraciones
Ejecuta:
```bash
npx prisma migrate dev --name init
```
Observa:
- Carpeta migrations/
- Archivos SQL generados
- Base de datos creada

### Tarea 2: Operaciones CRUD
Usa Prisma Client:
```javascript
const { PrismaClient } = require('@prisma/client');
const prisma = new PrismaClient();

// Create
await prisma.user.create({ data: { name: "Juan", email: "juan@email.com" } });
// Read
await prisma.user.findMany();
// Update
await prisma.user.update({ where: { id: 1 }, data: { name: "Juan Carlos" } });
// Delete
await prisma.user.delete({ where: { id: 1 } });
```

### Tarea 3: Integrar con Express
Conecta Prisma con tu API Express.

## Ejercicios Adicionales
- Practica con upsert
- Experimenta con createMany
