# Docker Compose Guide

## Introduction

Docker Compose is a tool used to define and run applications that contain multiple Docker containers. In this laboratory, Docker Compose was used to deploy a Nextcloud application together with a MariaDB database. Instead of starting each container separately, the configuration was written in a single `docker-compose.yml` file.

## What Does the `services:` Block Do?

The `services:` block defines the different containers that make up the application. In our Compose file, there are two services: `database` and `app`.

The `database` service uses the `mariadb:10.6` image and provides the database needed by Nextcloud. The `app` service uses the `nextcloud` image and provides the web/application tier. Docker Compose uses these service definitions to create and run the required containers.

## How Does the Nextcloud App Find the Database?

The Nextcloud application finds the MariaDB database using the environment variable:

```yaml
- MYSQL_HOST=database
```

The value `database` matches the name of the database service defined under `services:`. Docker Compose creates a network for the services, allowing containers to communicate with each other using their service names. Therefore, the Nextcloud container can use `database` as the hostname instead of needing to know the database container's IP address.

## `docker run` vs. `docker-compose up -d`

The `docker run` command is normally used to create and start an individual container. When an application requires several containers, the commands and configuration have to be entered separately.

`docker-compose up -d` reads the configuration from the `docker-compose.yml` file and creates and starts all the services defined in it. The `-d` option runs the containers in detached mode, allowing them to continue running in the background while the terminal remains available for other commands.

For this laboratory, `docker-compose up -d` was more convenient because it started both the Nextcloud application and MariaDB database using one command.

## References

1. Docker Documentation. **How Compose works.**
   https://docs.docker.com/compose/intro/

2. Docker Documentation. **Define and run multi-container applications with Docker Compose.**
   https://docs.docker.com/get-started/workshop/

3. Docker Documentation. **docker run reference.**
   https://docs.docker.com/reference/cli/docker/container/run/

4. Docker Documentation. **docker compose up.**
   https://docs.docker.com/reference/cli/docker/compose/up/

