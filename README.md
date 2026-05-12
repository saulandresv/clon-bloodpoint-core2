# BloodPoint API

Backend REST del sistema de gestión de donaciones de sangre, desarrollado como parte del proyecto de título **BloodPoint**.

> Implementación propia del backend original → [Camilink/BloodPoint-core](https://github.com/Camilink/BloodPoint-core)

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

## Relación con el proyecto original

Este repositorio es una implementación propia del backend del proyecto de título [BloodPoint](https://github.com/Camilink/BloodPoint), desarrollado en equipo en DuocUC. El frontend móvil correspondiente está en [clon-bloodpoint-app](https://github.com/saulandresv/clon-bloodpoint-app).