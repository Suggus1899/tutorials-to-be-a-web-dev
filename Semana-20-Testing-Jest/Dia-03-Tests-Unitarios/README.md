# Día 3: Tests Unitarios

En este día aprenderás a escribir tests unitarios efectivos.

## Contenido
- Matchers de Jest
- describe y it/test
- beforeEach y afterEach
- Tests asíncronos

## Tareas

### Tarea 1: Matchers comunes
Practica con matchers:
```javascript
expect(value).toBe(2);          // igualdad estricta
expect(value).toEqual({a: 1});  // igualdad profunda
expect(value).toBeTruthy();     // verdadero
expect(value).toContain('a');   // contiene
expect(fn).toThrow();           // lanza error
```

### Tarea 2: Organizar tests
Usa describe para agrupar:
```javascript
describe('Calculator', () => {
  describe('sum', () => {
    it('should add two numbers', () => { ... });
    it('should handle negative numbers', () => { ... });
  });
});
```

### Tarea 3: Tests asíncronos
Practica con async/await:
```javascript
test('async operation', async () => {
  const result = await fetchData();
  expect(result).toEqual({ data: 'value' });
});
```

## Ejercicios Adicionales
- Practica con setup y teardown
- Experimenta con test.each para tests parametrizados
