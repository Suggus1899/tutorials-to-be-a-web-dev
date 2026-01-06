# Día 4: Backend - Base de Datos

En este día configurarás la base de datos.

## Contenido
- Configurar Prisma
- Definir modelos
- Migraciones
- Seeds

## Tareas

### Tarea 1: Setup Prisma
Configura Prisma:
```bash
npm install prisma @prisma/client
npx prisma init
```

### Tarea 2: Definir modelos
Crea el schema según tu diseño:
- Modelos principales
- Relaciones
- Índices

### Tarea 3: Migraciones y seeds
Ejecuta:
```bash
npx prisma migrate dev --name init
```
Crea script de seed con datos iniciales.

## Ejercicios Adicionales
- Crea script de reset de BD
- Usa Prisma Studio para verificar
