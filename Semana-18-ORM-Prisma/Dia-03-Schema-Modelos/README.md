# Día 3: Schema y Modelos

En este día aprenderás a definir modelos en Prisma.

## Contenido
- Sintaxis de Prisma Schema
- Tipos de datos
- Campos obligatorios y opcionales
- Valores por defecto

## Tareas

### Tarea 1: Definir modelos básicos
Crea modelos en schema.prisma:
```prisma
model User {
  id        Int      @id @default(autoincrement())
  email     String   @unique
  name      String?
  createdAt DateTime @default(now())
}
```

### Tarea 2: Tipos de campos
Practica con diferentes tipos:
- String, Int, Float, Boolean
- DateTime
- @unique, @default
- Campos opcionales con ?

### Tarea 3: Múltiples modelos
Crea modelos para una aplicación:
- User
- Post
- Category

## Ejercicios Adicionales
- Experimenta con enums en Prisma
- Practica con campos Json
