# Checkpoint 5 – The Container Lifecycle

## Docker Container Lifecycle Commands

### 1. List Running Containers

```bash
docker ps
```

This command lists all currently running Docker containers.

### 2. Stop the Running Container

```bash
docker stop nginx-server
```

This command stops the running `nginx-server` container.

### 3. Verify the Container Is Stopped

```bash
docker ps
```

This command verifies that the `nginx-server` container is no longer running.

### 4. Remove the Container Completely

```bash
docker rm nginx-server
```

This command permanently removes the stopped `nginx-server` container from the Docker environment.

## References

* Docker. *docker container ls (docker ps).* Docker Docs.
  https://docs.docker.com/reference/cli/docker/container/ls/

* Docker. *docker container stop (docker stop).* Docker Docs.
  https://docs.docker.com/reference/cli/docker/container/stop/

* Docker. *docker container rm (docker rm).* Docker Docs.
  https://docs.docker.com/reference/cli/docker/container/rm/


