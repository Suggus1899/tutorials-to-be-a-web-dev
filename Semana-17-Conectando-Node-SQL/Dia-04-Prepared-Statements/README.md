# Día 4: Prepared Statements

En este día aprenderás sobre seguridad con prepared statements.

## Contenido
- Qué son prepared statements
- Prevenir SQL Injection
- Parámetros posicionales vs nombrados
- Mejores prácticas

## Tareas

### Tarea 1: Entender SQL Injection
Identifica el problema:
```javascript
// ❌ Vulnerable
const sql = `SELECT * FROM users WHERE name = '${name}'`;
// ✅ Seguro
const sql = `SELECT * FROM users WHERE name = ?`;
```

### Tarea 2: Usar prepared statements
Practica con parámetros:
- db.run("INSERT INTO users (name, email) VALUES (?, ?)", [name, email])
- db.get("SELECT * FROM users WHERE id = ?", [id])

### Tarea 3: Parámetros nombrados
Usa parámetros con nombre:
```javascript
db.run(
  "INSERT INTO users (name, email) VALUES ($name, $email)",
  { $name: name, $email: email }
);
```

## Ejercicios Adicionales
- Investiga otros vectores de ataque
- Practica validación de inputs
