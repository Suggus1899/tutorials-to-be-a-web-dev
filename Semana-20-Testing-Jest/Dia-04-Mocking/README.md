# Día 4: Mocking

En este día aprenderás a crear mocks y spies.

## Contenido
- jest.fn() para crear mocks
- jest.mock() para mockear módulos
- Spies para espiar funciones
- Cuándo usar mocks

## Tareas

### Tarea 1: Mock functions
Crea mocks básicos:
```javascript
const mockFn = jest.fn();
mockFn.mockReturnValue(42);
mockFn.mockImplementation((x) => x * 2);

// Verificar llamadas
expect(mockFn).toHaveBeenCalled();
expect(mockFn).toHaveBeenCalledWith(arg);
```

### Tarea 2: Mockear módulos
Mockea dependencias:
```javascript
jest.mock('./database');
const db = require('./database');

db.findUser.mockResolvedValue({ id: 1, name: 'Test' });
```

### Tarea 3: Spies
Espía funciones existentes:
```javascript
const spy = jest.spyOn(object, 'method');
// usa el método
expect(spy).toHaveBeenCalled();
spy.mockRestore();
```

## Ejercicios Adicionales
- Mockea llamadas HTTP
- Practica con mocks de timers
