# Día 2: Setup de Prisma

En este día configurarás Prisma en tu proyecto.

## Contenido
- Instalación de Prisma
- Inicialización del proyecto
- Configuración de conexión
- Prisma CLI

## Tareas

### Tarea 1: Instalar Prisma
Configura Prisma:
```bash
npm install prisma --save-dev
npm install @prisma/client
npx prisma init
```

### Tarea 2: Configurar conexión SQLite
Edita prisma/schema.prisma:
```prisma
datasource db {
  provider = "sqlite"
  url      = "file:./dev.db"
}

generator client {
  provider = "prisma-client-js"
}
```

### Tarea 3: Explorar Prisma CLI
Practica con comandos:
- npx prisma generate
- npx prisma db push
- npx prisma studio
- npx prisma format

## Ejercicios Adicionales
- Configura también para PostgreSQL (local o cloud)
- Explora las opciones de schema.prisma
