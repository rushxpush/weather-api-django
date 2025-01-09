## Weather Api Django
A Django-based microservice for providing weather data using PostgreSQL. This service is part of a larger distributed application.

### Prerequisites
- Docker and Docker Compose
- Python 3.9+ (if running locally)
- PostgresSQL database

### Running with Docker
TO-DO

2. Run the Container
```bash
docker run --env-file .env -p 8000:8000 weather-api-django
```

### If not using Docker (manual installation)
1. Clone the repository:
```bash
git clone https://github.com/rushxpush/weather-api-django.git
```

2. Create a virtual environment and activate it:
```bash
# Linux
source venv/bin/activate
# Windows
venv/Scripts/activate # I need to check this
```

3. Install dependencies
```bash
pip install -r requirements.txt
```

4. Apply migrations
```bash
python manage.py migrate
```

5. Run the development server
```bash
python manage.py runserver
```


### Environment variables
Create a '.env' file in the project root with the following variables:

DEBUG=True
POSTGRES_USERNAME=<YOUR_DATABASE_USERNAME>
POSTGRES_PASSWORD=<YOUR_DATABASE_PASSWORD>
POSTGRES_PORT=5430
POSTGRES_HOST=localhost

### Project Structure
- `weather_project/`: The main Django project containing settings and configurations.
- `weather_api/`: The Django app containing the API logic and models.

### Frequently used commands
- Run the development server:
```bash
python manage.py runserver
```

- Create a new migration:
```bash
python manage.py makemigrations
```

- Apply migrations:
```bash
python manage.py migrate
```

- Run tests:
```bash
python manage.py test
```