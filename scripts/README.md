# 🔧 Scripts de Utilidad

Este directorio contiene scripts para automatizar tareas comunes.

## 📋 Scripts Disponibles

### setup.sh
Configura el entorno de desarrollo completo
```bash
./scripts/setup.sh
```

### deploy.sh
Despliega la aplicación
```bash
./scripts/deploy.sh [staging|production]
```

### backup.sh
Realiza backup de la base de datos
```bash
./scripts/backup.sh
```

### migrate.py
Ejecuta migraciones de datos
```bash
python scripts/migrate.py
```

## 🚀 Uso

Asegúrate de dar permisos de ejecución:
```bash
chmod +x scripts/*.sh
```