# Día 6: Queries Avanzadas

En este día aprenderás queries avanzadas con Prisma.

## Contenido
- Filtros y ordenamiento
- Include y select
- Agregaciones
- Transacciones

## Tareas

### Tarea 1: Filtros
Practica con where:
```javascript
await prisma.user.findMany({
  where: {
    email: { contains: "gmail" },
    createdAt: { gte: new Date("2024-01-01") }
  }
});
```

### Tarea 2: Include y Select
Carga relaciones:
```javascript
// Include - carga relación completa
await prisma.user.findMany({ include: { posts: true } });

// Select - campos específicos
await prisma.user.findMany({ select: { name: true, email: true } });
```

### Tarea 3: Agregaciones
Usa funciones de agregación:
```javascript
await prisma.post.count();
await prisma.post.aggregate({ _avg: { views: true } });
await prisma.post.groupBy({ by: ['authorId'], _count: true });
```

## Ejercicios Adicionales
- Practica con transacciones ($transaction)
- Experimenta con raw queries (prisma.$queryRaw)
