# Día 3: Componentes

En este día aprenderás a crear componentes.

## Contenido
- Componentes funcionales
- Composición
- Importar/exportar
- Organización

## Tareas

### Tarea 1: Crear componentes
Crea componentes básicos:
```jsx
// Header.jsx
function Header() {
  return <header><h1>Mi App</h1></header>;
}
export default Header;
```

### Tarea 2: Composición
Usa componentes dentro de otros:
```jsx
import Header from './Header';
import Footer from './Footer';

function App() {
  return (
    <>
      <Header />
      <main>Contenido</main>
      <Footer />
    </>
  );
}
```

### Tarea 3: Organización
Organiza en carpetas:
```
src/
  components/
    Header/
      Header.jsx
      Header.css
    Footer/
      Footer.jsx
```

## Ejercicios Adicionales
- Crea componentes más complejos
- Practica con barrel exports (index.js)
