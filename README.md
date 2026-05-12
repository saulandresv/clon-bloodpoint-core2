> [!IMPORTANT]
> Implementación propia del backend del proyecto de título **BloodPoint**, desarrollado en equipo en DuocUC.
> Ver repositorio original: [Camilink/BloodPoint-core](https://github.com/Camilink/BloodPoint-core)

# BloodPoint API

Backend REST del sistema de gestión y promoción de donaciones de sangre.

## Stack

| Categoría | Tecnología |
|-----------|-----------|
| Framework | Django 5.2 + Django REST Framework |
| Auth | JWT + CORS |
| Tareas async | Celery + Redis |
| Analytics | Apache Superset 4.1 |
| Base de datos | PostgreSQL |
| Notificaciones push | Firebase Admin SDK |
| Almacenamiento | Cloudinary |
| Geolocalización | Geopy |
| Servidor | Gunicorn + Whitenoise |
| Deploy | Docker · Render · Heroku |

## Mis contribuciones

- **Auth completa:** login con token JWT, soporte CORS, headers Authorization, login por email (representantes) y RUT (donantes)
- **Perfiles:** endpoint `/profile/` para ver y editar datos del donante (email, RUT)
- **Donaciones:** registro de donaciones, historial por donante, registro vía QR
- **Campañas:** crear campaña, validar campaña, listar campañas activas, solicitudes de campaña
- **Representantes:** endpoints GET `/representantes/<id>`, generación automática de RUT único
- **Sistema de logros:** modelos, migraciones, services, serializers y seed de achievements (`init_achievements.py`, migración de población)
- **Chatbot:** integración del chatbot (`BPCB.json`, views)
- **Notificaciones:** push notifications server-side vía Firebase Admin
- **Deploy:** configuración Gunicorn en Procfile

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