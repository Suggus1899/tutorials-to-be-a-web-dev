# Día 4: Relaciones en Prisma

En este día aprenderás a definir relaciones entre modelos.

## Contenido
- Relaciones One-to-Many
- Relaciones Many-to-Many
- @relation directive
- Campos de relación

## Tareas

### Tarea 1: Relación One-to-Many
Define relación User → Posts:
```prisma
model User {
  id    Int    @id @default(autoincrement())
  posts Post[]
}

model Post {
  id       Int  @id @default(autoincrement())
  author   User @relation(fields: [authorId], references: [id])
  authorId Int
}
```

### Tarea 2: Relación Many-to-Many
Define relación Posts ↔ Tags:
```prisma
model Post {
  id   Int   @id @default(autoincrement())
  tags Tag[]
}

model Tag {
  id    Int    @id @default(autoincrement())
  posts Post[]
}
```

### Tarea 3: Schema completo
Crea un schema con múltiples relaciones:
- Users, Posts, Comments, Tags

## Ejercicios Adicionales
- Experimenta con relaciones self-referencing
- Practica con onDelete y onUpdate
