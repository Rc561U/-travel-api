# Travel assistant API (Python+Django+DRF)

### 
> ### Technologies used:
>
> - Docker & Docker-Compose
> - Django
> - Django Rest Framework


## Pre installation

### 1. Set global environment variables
```bash
cp .env-example .env
```
### 2 Create virtual local-environment
```bash
python3 -m venv venv
```
```bash
source venv/bin/activate
```

<hr>
## Installation
### 1. Start application
```bash
docker-compose up --build
```

### 2. Make database migrations
```bash
docker-compose exec webapp bash
``` 
```bash
cd src/
``` 
```bash
python manage.py makemigrations
``` 
```bash
python manage.py migrate
``` 

