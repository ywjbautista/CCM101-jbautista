# Laboratory 07 - Cloud Operations Engineer

## Mission Overview

This laboratory focused on checking Linux host resources and monitoring a containerized Nginx website. The activity involved checking system memory and disk storage, deploying a container, generating web traffic, reviewing application logs, and observing container metrics.

## Objectives

- Check the host's memory and disk capacity.
- Observe running processes using `top`.
- Deploy an Nginx container using Docker.
- Generate successful HTTP requests and a 404 response.
- Inspect application logs and monitor container resource usage.

## Monitoring Commands Executed

- `free -h` - checks memory usage and availability.
- `df -h /` - checks root filesystem storage.
- `top` - displays running processes and CPU activity.
- `docker run -d --name client-website -p 8080:80 nginx` - starts the Nginx container.
- `curl` - sends HTTP requests to the website.
- `docker logs client-website` - displays container logs.
- `docker stats` - displays live container resource metrics.

## Skills Learned

I practiced checking Linux system resources, deploying an Nginx container, generating HTTP requests, identifying a 404 response in application logs, and monitoring CPU and memory usage with Docker.
