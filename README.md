> [!IMPORTANT]
> Implementación propia del backend del proyecto de título **BloodPoint**, desarrollado en equipo en DuocUC.
> Ver repositorio original: [Camilink/BloodPoint-core](https://github.com/Camilink/BloodPoint-core)

# BloodPoint API

Backend REST del sistema de gestión de donaciones de sangre, desarrollado como parte del proyecto de título **BloodPoint**.

## Stack

- **Framework:** Django 4 + Django REST Framework
- **Tareas async:** Celery + Redis
- **Analytics:** Apache Superset
- **Almacenamiento:** Cloudinary
- **Deploy:** Render / Heroku (Docker)

## Funcionalidades

- Autenticación y gestión de usuarios donantes
- API REST para registro de donaciones
- Notificaciones asíncronas vía Celery
- Dashboard de analytics con Apache Superset
- Upload de imágenes a Cloudinary

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