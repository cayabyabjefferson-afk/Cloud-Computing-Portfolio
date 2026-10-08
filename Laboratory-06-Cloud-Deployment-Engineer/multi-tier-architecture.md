# Two-Tier Architecture

A **Two-Tier Architecture** is a system design that separates an application into two main tiers: the **Web/Application Tier** and the **Database Tier**. The two tiers have different responsibilities and communicate with each other to provide the application’s services. Separating responsibilities helps make the system easier to manage, maintain, and scale.

## The Web/Application Tier

The **Web/Application Tier** is responsible for interacting with users and handling application requests. It serves the user interface, receives HTTP requests from users, processes application logic, and communicates with the database when information needs to be retrieved or stored. In a containerized environment, the web/application component can run in its own Docker container.

## The Database Tier

The **Database Tier** is responsible for storing and managing the application's persistent data. This can include user accounts, login information, product records, transactions, and other information that needs to be saved even after the application is restarted. A database can run in its own container and communicate with the application container through a Docker network.

## Why Separate Them?

It is better to place the web server and database in **two separate containers** because each container can focus on one main responsibility. This provides isolation and allows the web application and database to be managed, updated, restarted, or scaled independently without unnecessarily affecting the other component. Docker recommends using separate containers for different application components, such as the frontend, backend, and database.

## References

1. Microsoft Learn. **N-tier Architecture Style**.
   [Microsoft Azure Architecture Center](https://learn.microsoft.com/azure/architecture/guide/architecture-styles/n-tier?utm_source=chatgpt.com)

2. Docker Documentation. **What is a Container?**
   [Docker Documentation – What is a Container?](https://docs.docker.com/get-started/docker-concepts/the-basics/what-is-a-container?utm_source=chatgpt.com)

3. Docker Documentation. **Multi-container Applications**.
   [Docker Documentation – Multi-container Applications](https://docs.docker.com/get-started/docker-concepts/running-containers/multi-container-applications/?utm_source=chatgpt.com)

4. Docker Documentation. **Use Containerized Databases**.
   [Docker Documentation – Use Containerized Databases](https://docs.docker.com/guides/databases/?utm_source=chatgpt.com)

