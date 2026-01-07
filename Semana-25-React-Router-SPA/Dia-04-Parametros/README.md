# Día 4: Parámetros de Ruta

En este día aprenderás a usar parámetros en rutas.

## Contenido
- Parámetros dinámicos (:id)
- useParams hook
- Query strings
- useSearchParams

## Tareas

### Tarea 1: Parámetros de ruta
Define rutas con parámetros:
```jsx
<Route path="/users/:id" element={<UserDetail />} />
```
Accede al parámetro:
```jsx
import { useParams } from 'react-router-dom';

function UserDetail() {
  const { id } = useParams();
  return <div>Usuario: {id}</div>;
}
```

### Tarea 2: Múltiples parámetros
Usa varios parámetros:
```jsx
<Route path="/posts/:category/:id" element={<Post />} />

const { category, id } = useParams();
```

### Tarea 3: Query strings
Usa useSearchParams:
```jsx
import { useSearchParams } from 'react-router-dom';

function Search() {
  const [searchParams, setSearchParams] = useSearchParams();
  const query = searchParams.get('q');
  // URL: /search?q=react
}
```

## Ejercicios Adicionales
- Crea una página de detalle de producto
- Practica con filtros en URL
