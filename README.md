# Librería Online

Aplicación web construida con Django y Django REST Framework. Permite gestionar un catálogo de libros, autores, editoriales, y pedidos.

## Características principales

- Vista pública con listado de libros disponibles.
- API RESTful para libros, autores, editoriales, categorías y carritos.
- Autenticación JWT.
- Documentación automática con Swagger y Redoc.
- Django Debug Toolbar para análisis de rendimiento.

## Documentación

- Swagger UI: [http://127.0.0.1:8000/swagger/](http://127.0.0.1:8000/swagger/)
- Redoc: [http://127.0.0.1:8000/redoc/](http://127.0.0.1:8000/redoc/)
- Esquema OpenAPI JSON: [http://127.0.0.1:8000/schema/](http://127.0.0.1:8000/schema/)

## Instalación

```bash
python -m venv venv
source venv/bin/activate  # en Windows: venv\Scripts\activate
pip install -r requirements.txt
```

## Ejecutar localmente

```bash
python manage.py migrate
python manage.py runserver
```

## Variables de entorno

- `.env` con clave `SECRET_KEY` y `DEBUG=True`

## Tests

```bash
pytest
```