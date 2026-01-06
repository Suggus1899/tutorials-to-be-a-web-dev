# Día 5: Repository Pattern

En este día aprenderás el patrón Repository para organizar acceso a datos.

## Contenido
- Qué es el Repository Pattern
- Separar lógica de datos
- Crear repositorios
- Testabilidad

## Tareas

### Tarea 1: Crear un repository
Crea userRepository.js:
```javascript
const db = require('./database');

module.exports = {
  async findAll() { ... },
  async findById(id) { ... },
  async create(data) { ... },
  async update(id, data) { ... },
  async delete(id) { ... }
};
```

### Tarea 2: Usar repository en service
Conecta las capas:
- Service llama al Repository
- Repository ejecuta las queries
- Controller usa el Service

### Tarea 3: Múltiples repositories
Crea repositories para diferentes entidades:
- productRepository.js
- orderRepository.js
- categoryRepository.js

## Ejercicios Adicionales
- Implementa un BaseRepository con operaciones comunes
- Practica con inyección de dependencias
