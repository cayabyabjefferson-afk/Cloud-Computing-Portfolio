# Laboratory-06-Cloud-Deployment-Engineer

## Mission Overview

This laboratory focused on deploying a multi-container cloud application using Docker Compose. A two-tier architecture was created using Nextcloud as the web/application tier and MariaDB as the database tier. The infrastructure was defined in a `docker-compose.yml` file and deployed using Docker Compose.

## Objectives

* Understand the basic concept of two-tier architecture.
* Identify the roles of the web/application tier and database tier.
* Create a Docker Compose configuration file.
* Deploy multiple containers using Docker Compose.
* Connect a Nextcloud application container to a MariaDB database container.
* Access the Nextcloud web interface through port 8080.
* Start and stop a multi-container application using Docker Compose.
* Document the deployment process and commands used.

## Commands Executed

The following commands were used during the laboratory:

```bash
mkdir nextcloud-deployment
cd nextcloud-deployment
nano docker-compose.yml
docker-compose up -d
docker-compose ps
docker-compose logs --tail=50
docker-compose down
```

The `mkdir` command created the project directory, while `cd` moved into the directory. The `nano` command was used to create and edit the Docker Compose YAML file.

The `docker-compose up -d` command deployed the services in the background. `docker-compose ps` was used to check the status of the containers. `docker-compose logs` was used to view container logs when troubleshooting. Finally, `docker-compose down` stopped and removed the containers and network created by the Compose deployment.

## Skills Learned

Through this laboratory, I learned how to design a simple two-tier application architecture and represent it using Docker Compose. I learned how multiple containers can communicate using Docker Compose service names and environment variables.

I also learned how to deploy, inspect, troubleshoot, and shut down a multi-container application. Most importantly, I gained practical experience deploying Nextcloud with MariaDB and learned how infrastructure can be described as configuration instead of being created manually through many separate commands.

## References

1. Docker Documentation. **Docker Compose.**
   https://docs.docker.com/compose/

2. Docker Documentation. **Docker Compose CLI Reference.**
   https://docs.docker.com/reference/cli/docker/compose/

3. Nextcloud Documentation. **Installation.**
   https://docs.nextcloud.com/server/latest/admin_manual/installation/

