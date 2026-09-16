# Laboratory Activity 4 - The Cloud-Native Engineer

## Mission Overview

This laboratory activity gave me hands-on experience with Docker and containerization. Instead of only comparing Virtual Machines and Containers, I was able to use Docker commands in KillerCoda and deploy an actual Nginx web server. I also practiced managing the container from the time it was created until it was removed.

## Objectives

- Understand how Virtual Machines and Containers differ.
- Practice using Docker commands in a Linux environment.
- Pull and run a container image.
- Deploy and test an Nginx web server.
- Understand port mapping and the container lifecycle.
- Document the activity using Markdown and GitHub.

## Docker Commands Executed

`docker --version` - Checked the Docker version installed in the environment.

`docker ps` - Displayed the containers that were currently running.

`docker pull nginx` - Downloaded the official Nginx image.

`docker run -d --name nginx-web -p 8080:80 nginx` - Started the Nginx container and mapped the required ports.

`curl http://localhost:8080` - Tested if the Nginx server was responding.

`docker stop nginx-web` - Stopped the Nginx container.

`docker ps -a` - Displayed running and stopped containers.

`docker rm nginx-web` - Removed the stopped Nginx container.

## Skills Learned

I learned how basic Docker commands work together when deploying and managing a container. I was able to download an image, start a containerized web server, test it, check its status, stop it, and remove it. I also practiced documenting my commands and results in my GitHub portfolio.

## Challenges Encountered

At first, I needed to understand the purpose of each Docker command instead of simply entering them in the terminal. Port mapping was also new to me because I had to understand the connection between port 8080 on the host and port 80 inside the container. Seeing the actual output of the commands helped me understand the process more clearly.
