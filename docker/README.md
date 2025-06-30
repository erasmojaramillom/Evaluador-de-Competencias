# 🐳 Docker Configuration

## Estructura

```
docker/
├── Dockerfile.frontend
├── Dockerfile.backend
├── docker-compose.yml
├── docker-compose.dev.yml
└── docker-compose.prod.yml
```

## 🚀 Inicio Rápido

### Desarrollo
```bash
docker-compose -f docker/docker-compose.dev.yml up
```

### Producción
```bash
docker-compose -f docker/docker-compose.prod.yml up -d
```

## 📋 Servicios

- **frontend**: Aplicación React (puerto 3000)
- **backend**: API FastAPI (puerto 8000)
- **postgres**: Base de datos PostgreSQL
- **redis**: Cache y cola de tareas
- **nginx**: Proxy reverso (producción)

## 🔧 Comandos Útiles

```bash
# Ver logs
docker-compose logs -f [servicio]

# Ejecutar comandos en contenedor
docker-compose exec backend python manage.py migrate

# Reconstruir imágenes
docker-compose build --no-cache
```