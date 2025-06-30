# 🧪 Testing

## Estructura de Tests

```
tests/
├── unit/              # Tests unitarios
├── integration/       # Tests de integración
├── e2e/              # Tests end-to-end
└── fixtures/         # Datos de prueba
```

## Ejecutar Tests

### Backend (Python)
```bash
# Todos los tests
pytest

# Con cobertura
pytest --cov=app

# Tests específicos
pytest tests/unit/test_services.py
```

### Frontend (JavaScript)
```bash
# Todos los tests
npm test

# Modo watch
npm test -- --watch

# Con cobertura
npm test -- --coverage
```

## Escribir Tests

### Ejemplo Backend
```python
def test_evaluate_competency():
    result = evaluate_competency(user_id=1, competency_id=1)
    assert result.score >= 0
    assert result.score <= 100
```

### Ejemplo Frontend
```javascript
test('renders evaluation form', () => {
  render(<EvaluationForm />);
  expect(screen.getByText(/Iniciar Evaluación/i)).toBeInTheDocument();
});
```