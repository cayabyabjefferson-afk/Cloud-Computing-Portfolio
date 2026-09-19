

## Mission Overview

This laboratory introduces the basic concepts and practices of cloud-native application deployment using Docker. The activity focuses on understanding the difference between virtual machines and containers, launching a Docker environment, deploying an Nginx web server, and managing the container lifecycle.

## Objectives

* Understand the differences between Virtual Machines and Containers.
* Launch and verify a Docker environment.
* Pull an official Nginx image from Docker Hub.
* Deploy an Nginx container using Docker.
* Access the web server through a local HTTP request.
* Learn how to list, stop, verify, and remove Docker containers.
* Develop basic skills in managing containerized applications.

## Docker Commands Executed

### Checkpoint 3 – Enter the Docker Playground

```bash
docker --version
docker info
docker ps
```

### Checkpoint 4 – Deploy Your First Container

```bash
docker pull nginx
docker run -d -p 8080:80 --name nginx-server nginx
docker ps
curl http://localhost:8080
```

### Checkpoint 5 – The Container Lifecycle

```bash
docker ps
docker stop nginx-server
docker ps
docker rm nginx-server
```

## Skills Learned

Through this laboratory, I learned how to use basic Docker commands and manage containers from the terminal. I learned how to download Docker images from Docker Hub and create containers from those images. I also learned how to map ports so that a web application running inside a container can be accessed from the host environment. In addition, I learned how to check, stop, and remove containers as part of the Docker container lifecycle.

## Challenges Encountered

One challenge was becoming familiar with Docker commands and understanding what each command does. Another challenge was ensuring that the Nginx container was running correctly and that port 8080 was properly mapped to port 80 inside the container. I also needed to verify the container status before stopping and removing it. These challenges helped me become more comfortable with using the Docker command line and managing containerized applications.

## Screenshots

The screenshots for the laboratory activities are stored in the `screenshots` folder.

* `docker-version.png` – Docker installation and environment verification
* `nginx-running.png` – Successful Nginx HTTP request
* `container-lifecycle.png` – Docker container lifecycle commands

