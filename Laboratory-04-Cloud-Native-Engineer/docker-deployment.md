# Docker Deployment and Container Lifecycle

## Nginx Deployment

### Pulling the Nginx Image

`docker pull nginx`

I used this command to get the official Nginx image that I needed for the web server.

### Running the Container

`docker run -d --name nginx-web -p 8080:80 nginx`

This started my Nginx container in the background and connected host port 8080 to port 80 inside the container.

### Testing Nginx

`curl http://localhost:8080`

I used this command to send a request to the web server and confirm that Nginx was responding successfully.

## Container Lifecycle

### Listing the Running Container

`docker ps`

This showed me which containers were currently active.

### Stopping the Container

`docker stop nginx-web`

This stopped my running Nginx container without removing it yet.

### Checking the Stopped Container

`docker ps -a`

This allowed me to check all containers and confirm that nginx-web had an Exited status.

### Removing the Container

`docker rm nginx-web`

This completely removed the stopped Nginx container from the Docker environment.
