# ModelDeveloper

A Django application for developing and managing developers' models.

## Requirements

- Python 3.8+
- Django 6.0.3
- PostgreSQL

## Installation

### 1. Clone the repository

```bash
git clone <repository-url>
cd ModelDeveloper
```

### 2. Install dependencies

```bash
pip install -r requirements.txt
```

### 3. Configure the environment

Create a `.env` file in the project root directory:

```
DB_NAME=your_database_name
DB_USER=your_database_user
DB_PASSWORD=your_database_password
DB_HOST=localhost
DB_PORT=5432
```

### 4. Run migrations

```bash
python manage.py migrate
```

### 5. Create a superuser

```bash
python manage.py createsuperuser
```

## Running the project

### Local development server

```bash
python manage.py runserver
```

The application will be available at: `http://127.0.0.1:8000/`

Admin panel: `http://127.0.0.1:8000/admin/`

## Project structure

```
ModelDeveloper/
├── manage.py              # Django management utility
├── requirements.txt       # Project dependencies
├── .env                   # Environment variables (do not commit!)
├── .gitignore            # Files to ignore in git
├── ModelDeveloper/       # Main application package
│   ├── __init__.py
│   ├── settings.py       # Django settings
│   ├── urls.py          # Application routes
│   ├── asgi.py          # ASGI configuration
│   └── wsgi.py          # WSGI configuration
```

## Technologies used

- **Django** - web application framework
- **PostgreSQL** - database
- **psycopg2** - PostgreSQL adapter for Python
- **django-environ** - environment variable management

## Development

### Create a new application

```bash
python manage.py startapp app_name
```

### Create migrations

```bash
python manage.py makemigrations
```

### Apply migrations

```bash
python manage.py migrate
```

## License

No license.

## Contact

For questions and suggestions, please open an issue in the repository.
