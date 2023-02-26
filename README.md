# docker-compose-python

This is a simple docker compose app using Flask.

1. Clone this repository.
```
git clone https://github.com/abohatyrov/docker-compose-python.git
cd docker-compose-python
```

2. Build the Docker images and start the containers:
```
docker-compose up
```
Now you can access the application at http://localhost

`docker-compose.yaml` defines two services, `frontend` and `backend`. The `frontend` service maps port 80 on the host to port 80 in the container, while the backend service maps port 5000 on the host to port 5000 in the container. These containers created in the same network so thay can communicate wuth each other.

`nginx.conf` is a configuration file for web server. It is a `frontend` that communicate with backend.
