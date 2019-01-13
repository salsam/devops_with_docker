# Ensuring that process is not ran as root

1. Go to docker file `backend-example-docker/Dockerfile` and remove `-R` flag from chown.
2. In this directory run `docker-compose build && docker-compose up`
3. Notice how backend fails to start due to missing permissions.

Similarly to ensure that frontend is ran as regular user replace `backend-example-docker` with `frontend-example-docker` in above instructions.