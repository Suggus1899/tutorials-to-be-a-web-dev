# Día 7: Práctica Integradora

En este día realizarás ejercicios que integran todos los conceptos de la semana.

## Contenido
- Repaso de Node.js y módulos
- Repaso de HTTP
- Repaso de File System
- Proyecto integrador

## Proyecto del Día

### Proyecto: API de Notas con Persistencia en Archivos

Crea un servidor que maneje notas guardadas en archivos JSON:

1. **Estructura de datos:**
   ```javascript
   const nota = {
     id: "uuid",
     titulo: "Mi nota",
     contenido: "Contenido de la nota",
     createdAt: "2024-01-15T10:30:00Z",
     updatedAt: "2024-01-15T10:30:00Z"
   };
   ```

2. **Endpoints a implementar:**
   - GET /notas → Lista todas las notas
   - GET /notas/:id → Obtiene una nota por ID
   - POST /notas → Crea una nueva nota
   - PUT /notas/:id → Actualiza una nota
   - DELETE /notas/:id → Elimina una nota

3. **Persistencia:**
   - Guarda las notas en un archivo notas.json
   - Lee el archivo al iniciar el servidor
   - Actualiza el archivo en cada operación

4. **Características adicionales:**
   - Genera IDs únicos para cada nota
   - Valida que título y contenido no estén vacíos
   - Maneja errores apropiadamente

## Tareas Adicionales

### Tarea 1: Búsqueda
Implementa búsqueda de notas por título o contenido.

### Tarea 2: Categorías
Agrega categorías a las notas y permite filtrar.

## Ejercicios de Repaso
- Revisa los conceptos que te costaron más durante la semana
- Practica los ejercicios que no completaste de días anteriores
