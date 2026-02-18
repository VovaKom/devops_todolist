# TodoApp Docker Image

Docker Hub: https://hub.docker.com/r/vovakomar/todoapp

## Build image
docker build --build-arg PYTHON_VERSION=3.10 -t todoapp:1.0.0 .

## Run container
docker run -p 8080:8080 todoapp:1.0.0

## Access in a browser
http://localhost:8080

## Additionally
- To manually run migrations:
  docker exec -it <container_id> python manage.py migrate
- When building, you can change the Python version via --build-arg PYTHON_VERSION=<version>