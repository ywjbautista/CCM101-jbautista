# Docker Compose Guide

## Services Block

The `services:` block defines the containers that make up the application.

The `database` service uses MariaDB as the database tier, while the `app` service uses Nextcloud as the application tier.

## MYSQL_HOST=database

The `MYSQL_HOST=database` setting tells the Nextcloud application where to find the MariaDB database.

The value `database` refers to the database service name in the Docker Compose file.

## Docker Run vs Docker Compose

`docker run` is used to create and run an individual container.

`docker-compose up -d` is used to start multiple services defined in a Docker Compose file. It is useful for multi-container applications because the services and their configuration are defined in one file.
