> [!IMPORTANT]
> Implementación propia del backend del proyecto de título **BloodPoint**, desarrollado en equipo en DuocUC.
> Ver repositorio original: [Camilink/BloodPoint-core](https://github.com/Camilink/BloodPoint-core)

# BloodPoint API

Backend REST del sistema de gestión y promoción de donaciones de sangre.

## Stack

| Categoría | Tecnología |
|-----------|-----------|
| Framework | Django 5.2 + Django REST Framework |
| Tareas async | Celery 5.5 + Redis |
| Analytics | Apache Superset 4.1 |
| Base de datos | PostgreSQL (psycopg2) |
| Notificaciones push | Firebase Admin SDK |
| Almacenamiento | Cloudinary |
| Geolocalización | Geopy |
| Data processing | Pandas + NumPy + PyArrow |
| Alertas | Slack SDK |
| Servidor | Gunicorn + Whitenoise |
| Deploy | Docker · Render · Heroku |

## Funcionalidades

- API REST para registro y gestión de donantes y donaciones
- Tareas asíncronas con Celery + Redis (notificaciones, reportes)
- Dashboard de analytics con Apache Superset integrado
- Notificaciones push server-side vía Firebase Admin
- Upload y gestión de imágenes con Cloudinary
- Geolocalización de puntos de donación con Geopy
- Alertas a Slack para eventos críticos
- Datos de prueba con Faker

## Instalación

```bash
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
```

**Con Docker:**
```bash
docker-compose up
```

## Frontend

App móvil correspondiente: [clon-bloodpoint-app](https://github.com/saulandresv/clon-bloodpoint-app)