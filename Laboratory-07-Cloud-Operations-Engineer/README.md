
# Laboratory 07 - Cloud Operations Engineer

## Mission Overview

This laboratory focused on checking Linux server resources and observing a containerized Nginx website. Linux commands and Docker tools were used to review system health, generate web requests, inspect application logs, and monitor container performance.

## Objectives

- Check the host's memory and disk capacity.
- Observe running processes and CPU activity.
- Deploy an Nginx web server using Docker.
- Generate successful HTTP requests and a 404 error.
- Review application logs and live container metrics.

## Monitoring Commands Executed

- `free -h` - check memory.
- `df -h /` - check root filesystem storage.
- `top` - observe processes and CPU activity.
- `docker run -d --name client-website -p 8080:80 nginx` - deploy Nginx.
- `curl` - send HTTP requests.
- `docker logs client-website` - view application logs.
- `docker stats` - monitor live container resource usage.

## Skills Learned

I practiced checking Linux system resources, starting a Docker container, generating web traffic, finding an HTTP error in application logs, and observing container CPU and memory usage.
