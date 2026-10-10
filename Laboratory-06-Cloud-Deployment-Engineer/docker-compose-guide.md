# Docker Compose Guide

## Introduction
Docker Compose is a tool used to define and manage applications that consist of multiple containers. It uses a YAML configuration file named `docker-compose.yml` to describe the application's services and their settings.

## What Does the `services:` Block Do?
The `services:` block defines the containers that make up the application. In this project, it contains two services: `database`, which uses the MariaDB 10.6 image, and `app`, which uses the Nextcloud image.

The database service defines environment variables for the database root password, database name, database user, and user password. The app service maps host port 8080 to container port 80 and receives the database connection settings through environment variables.

## How Does Nextcloud Find the Database?
The environment variable `MYSQL_HOST=database` tells Nextcloud to connect to the database service using the hostname `database`. Docker Compose creates a shared network for the services, allowing them to communicate using their service names.

## Docker Run vs. Docker Compose Up -d
The `docker run` command is commonly used to create and start an individual container by specifying its image and options directly in the terminal. In contrast, `docker-compose up -d` reads the Compose configuration and creates or starts all the defined services in the background.

Docker Compose makes multi-container deployments easier to repeat and maintain because the infrastructure configuration is stored in one file.

## Commands Used

```bash
mkdir nextcloud-deployment
cd nextcloud-deployment
nano docker-compose.yml
docker-compose up -d
docker-compose ps
docker-compose logs --tail=50
docker-compose down
```

If the environment uses the newer Compose plugin, the equivalent commands use `docker compose` with a space.

## Infrastructure as Code
Infrastructure as Code (IaC) means defining infrastructure through machine-readable configuration rather than relying entirely on manual setup. The Compose file documents the services and settings, making the deployment easier to reproduce, review, and maintain.

## Conclusion
This activity demonstrates how Docker Compose coordinates a web application and database in a two-tier architecture. It also highlights the importance of correct YAML formatting, service networking, and deployment verification.
