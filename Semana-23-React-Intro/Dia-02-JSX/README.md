# Día 2: JSX

En este día aprenderás la sintaxis JSX.

## Contenido
- Qué es JSX
- Expresiones en JSX
- Atributos y className
- Fragmentos

## Tareas

### Tarea 1: JSX básico
Practica escribiendo JSX:
```jsx
function App() {
  const nombre = "Juan";
  return (
    <div>
      <h1>Hola, {nombre}!</h1>
      <p>Bienvenido a React</p>
    </div>
  );
}
```

### Tarea 2: Expresiones
Usa expresiones JavaScript:
```jsx
const items = ['a', 'b', 'c'];
return <p>Tenemos {items.length} items</p>;
```

### Tarea 3: Atributos
Practica con atributos:
```jsx
<img src={imageUrl} alt="Descripción" />
<div className="container">
<button onClick={handleClick}>Click</button>
```

## Ejercicios Adicionales
- Experimenta con estilos inline
- Practica con fragmentos <></>
