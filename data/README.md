# 📊 Directorio de Datos

Este directorio contiene datasets y modelos utilizados por el sistema.

## 📁 Estructura

```
data/
├── raw/               # Datos sin procesar
├── processed/         # Datos procesados
├── models/           # Modelos entrenados
└── sample/           # Datos de ejemplo
```

## ⚠️ Importante

- No subir datos sensibles o privados
- Los archivos grandes deben usar Git LFS
- Mantener documentación de cada dataset
- Seguir estándares de nombrado consistentes

## 📝 Formato de Datos

### Competencias
```json
{
  "id": "string",
  "name": "string",
  "category": "string",
  "level": "integer",
  "description": "string"
}
```

### Evaluaciones
```json
{
  "id": "string",
  "user_id": "string",
  "competency_id": "string",
  "score": "float",
  "timestamp": "datetime"
}
```