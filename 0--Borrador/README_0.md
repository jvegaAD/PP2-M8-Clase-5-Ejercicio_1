
# Proyecto Backend - API de Libros

Este es un backend desarrollado con Django y Django REST Framework que expone una API para gestionar un catálogo de libros. Incluye funcionalidades como JWT para autenticación, documentación interactiva con Swagger y Redoc, y configuración para pruebas con Pytest.

---

## 📅 Requisitos

- Python 3.11+
- pip
- Virtualenv (recomendado)

---

## 🔧 Instalación local

1. Clonar el repositorio y acceder a la carpeta del proyecto:

```bash
cd ruta/al/proyecto/miproyecto
```

2. Crear entorno virtual:

```bash
python -m venv venv
source venv/bin/activate  # Linux/macOS
o bien:
venv\Scripts\activate     # Windows
```

3. Instalar dependencias:

```bash
pip install -r requirements.txt
```

4. Aplicar migraciones:

```bash
python manage.py migrate
```

5. Iniciar servidor:

```bash
python manage.py runserver
```

---

## 🔐 Autenticación JWT

- Obtener token:
  - `POST /api/token/`
- Refrescar token:
  - `POST /api/token/refresh/`
- Verificar token:
  - `POST /api/token/verify/`

---

## 🔍 Documentación interactiva

- Swagger UI: [http://127.0.0.1:8000/swagger/](http://127.0.0.1:8000/swagger/)
- Redoc: [http://127.0.0.1:8000/redoc/](http://127.0.0.1:8000/redoc/)
- OpenAPI JSON: [http://127.0.0.1:8000/schema/](http://127.0.0.1:8000/schema/)

---

## 📂 Estructura del proyecto

```
.
├── myproject/            # Configuración principal de Django
├── myapp/                # App principal con modelos, vistas y urls
├── web/                  # Frontend opcional
├── staticfiles/          # Archivos estáticos
├── data/                 # CSV para precarga de datos
├── requirements.txt      # Dependencias
├── manage.py             # Entrada al proyecto
```

---

## 🧪 Pruebas

```bash
pytest
```

---

## 🚫 Error de prueba para Sentry

Ruta incluida para probar errores:

```txt
GET /sentry-debug/
```

---

Este proyecto usa `drf-spectacular` para la generación de esquemas OpenAPI automáticos y documentación profesional.
