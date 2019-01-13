# Connecting frontend and backend

## Building

Build frontend app with updated Dockerfile `front_Dockerfile`

```bash
frontend-example-docker $ docker build -t frontend_17 .
```

and backend app with updated Dockerfile `back_Dockerfile`

```bash
backend-example-docker $ docker build -t backend_17 .
```

## Running

Assuming frontend image is built with tag `frontend_17` and backend with tag `backend_17` as above:

1. Run backend with `$ docker run -d -v $(pwd)/logs.txt:/backend-example-docker/logs.txt --name=backend_17 -p 8000:8000 backend_17`
2. Run frontend with `$ docker run -d --name=frontend_17 -p 5000:5000 frontend_17`