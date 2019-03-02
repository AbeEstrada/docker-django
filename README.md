### Build image

```
docker-compose build
```

### Create project

```
docker-compose run django django-admin startproject project_name .
```

### Create app

```
docker-compose run django python manage.py startapp app_name
```

### Add app to project `./app/project_name/settings.py`

```
INSTALLED_APPS = [
    'django.contrib.admin',
    'django.contrib.auth',
    'django.contrib.contenttypes',
    'django.contrib.sessions',
    'django.contrib.messages',
    'django.contrib.staticfiles',
    'app_name',
]
```

### Development

```
docker-compose up -d
```

```
docker-compose stop
```
