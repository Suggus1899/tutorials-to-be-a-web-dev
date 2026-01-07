# Día 2: Conceptos de Seguridad

En este día aprenderás conceptos de seguridad para autenticación.

## Contenido
- Hash de contraseñas
- bcrypt
- Salt y rounds
- Nunca guardar contraseñas en texto plano

## Tareas

### Tarea 1: Instalar bcrypt
Configura bcrypt:
```bash
npm install bcrypt
```

### Tarea 2: Hashear contraseñas
Practica:
```javascript
const bcrypt = require('bcrypt');
const saltRounds = 10;

// Hashear
const hash = await bcrypt.hash('password123', saltRounds);

// Comparar
const match = await bcrypt.compare('password123', hash);
```

### Tarea 3: Configurar salt rounds
Entiende:
- Qué es el salt
- Por qué importan los rounds
- Balance entre seguridad y performance

## Ejercicios Adicionales
- Investiga otros algoritmos (argon2)
- Practica con timing attacks y su prevención
