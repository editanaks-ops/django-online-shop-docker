## Docker Support

Проект контейнеризирован с использованием Docker.

### Build Docker image

```bash
docker build -t django-project .
```

### Run container

```bash
docker run -d --name django-container -p 8000:8000 django-project
```

### Apply migrations

```bash
docker exec django-container python manage.py migrate
```

### Check containers

```bash
docker ps -a
```

### Open project

```text
http://localhost:8000
```