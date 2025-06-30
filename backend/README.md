# Backend - Evaluador de Competencias

API REST para el sistema de evaluación de competencias.

## 🚀 Stack Tecnológico

- Python 3.9+
- FastAPI
- SQLAlchemy
- PostgreSQL
- Redis
- Celery

## 📁 Estructura

```
backend/
├── app/
│   ├── api/           # Endpoints API
│   ├── core/          # Configuración core
│   ├── models/        # Modelos de datos
│   ├── services/      # Lógica de negocio
│   ├── schemas/       # Pydantic schemas
│   └── utils/         # Utilidades
├── tests/             # Pruebas
├── alembic/           # Migraciones DB
└── requirements.txt   # Dependencias
```

## 🛠️ Instalación

```bash
python -m venv venv
source venv/bin/activate  # Linux/Mac
# o
venv\Scripts\activate  # Windows

pip install -r requirements.txt
```

## 🔧 Comandos

```bash
# Desarrollo
uvicorn app.main:app --reload

# Migraciones
alembic upgrade head

# Tests
pytest

# Celery worker
celery -A app.celery worker --loglevel=info
```