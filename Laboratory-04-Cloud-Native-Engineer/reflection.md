# Checkpoint 7 – Mission Reflection

In this laboratory, I learned that Docker containers can be started much faster than setting up a traditional Virtual Machine. A Virtual Machine needs to boot an entire operating system, while a container runs an application using the host system's kernel. Because of this, starting a Docker container can take only seconds, while installing and starting an operating system on a VM generally requires more time and resources. This makes containers useful when applications need to be deployed quickly and consistently.

Port mapping, such as `-p 8080:80`, is necessary because the web server inside the container is isolated from the host system. In our activity, Nginx listens on port 80 inside the container, while port 8080 is used on the host. Docker forwards requests from the host's port 8080 to the container's port 80, allowing us to access Nginx using `http://localhost:8080`.

When `docker rm` is used, the container itself is removed. Any data stored only in the container's writable layer can be lost when the container is removed, so important data should be stored using Docker volumes or other persistent storage. Docker's documentation explains that volumes can be managed separately from containers.

Containerization also changes how developers and IT operations teams work together. Developers can package an application with its dependencies into a container, while operations teams can run the same container consistently across different environments. This supports DevOps practices by making deployment, testing, and application management more consistent.

My GitHub portfolio is also evolving as I document each laboratory activity. I am adding Markdown files, screenshots, Docker commands, reflections, and references to organize my work. GitHub provides a README to explain a project's purpose and files, while repository history allows changes to be tracked over time.

## References

* Docker Docs. **Port publishing and mapping.**
  [Docker Documentation – Port publishing and mapping](https://docs.docker.com/engine/network/port-publishing/?utm_source=chatgpt.com)

* Docker Docs. **Publishing and exposing ports.**
  [Docker Documentation – Publishing and exposing ports](https://docs.docker.com/get-started/docker-concepts/running-containers/publishing-ports/?utm_source=chatgpt.com)

* Docker Docs. **docker container rm.**
  [Docker Documentation – docker container rm](https://docs.docker.com/reference/cli/docker/container/rm/?utm_source=chatgpt.com)

* GitHub Docs. **About README files.**
  [GitHub Documentation – About README files](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-readmes?utm_source=chatgpt.com)

