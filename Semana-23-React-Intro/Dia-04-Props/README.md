# Día 4: Props

En este día aprenderás a pasar datos con props.

## Contenido
- Qué son las props
- Pasar props
- Destructuring de props
- Props children

## Tareas

### Tarea 1: Pasar props
Pasa datos a componentes:
```jsx
function Saludo({ nombre }) {
  return <h1>Hola, {nombre}!</h1>;
}

// Uso
<Saludo nombre="María" />
```

### Tarea 2: Múltiples props
Pasa varias props:
```jsx
function UserCard({ nombre, email, avatar }) {
  return (
    <div className="card">
      <img src={avatar} alt={nombre} />
      <h2>{nombre}</h2>
      <p>{email}</p>
    </div>
  );
}
```

### Tarea 3: Children
Usa props.children:
```jsx
function Card({ children }) {
  return <div className="card">{children}</div>;
}

<Card>
  <h2>Título</h2>
  <p>Contenido</p>
</Card>
```

## Ejercicios Adicionales
- Practica con default props
- Experimenta con PropTypes
