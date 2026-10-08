
# Mission Reflection

Writing a `docker-compose.yml` file makes a cloud engineer's job easier because the configuration for multiple containers can be written and saved in one file. Instead of manually typing many `docker run` commands and remembering every option, the engineer can use `docker-compose up -d` to deploy the entire application. This also makes the deployment easier to repeat on another machine because the configuration is already documented.

I learned that YAML is very sensitive to indentation. An indentation error, such as using a Tab instead of spaces or placing a service at the wrong level, can cause Docker Compose to reject the file. During this laboratory, I experienced a Compose configuration error involving the `app` service. This helped me understand that proper YAML formatting is important because the indentation determines the structure and relationship between configuration items.

We used environment variables such as `MYSQL_PASSWORD`, `MYSQL_DATABASE`, and `MYSQL_USER` to provide configuration values to the containers. Environment variables allow the application and database settings to be passed to the containers without placing those values directly inside the application code. In our Compose file, `MYSQL_HOST=database` also allowed the Nextcloud application to find the database service using its Compose service name.

It was impressive to deploy a cloud storage system such as Nextcloud within a few minutes. The experience showed me how containers and automation can make application deployment much faster than installing and configuring every component manually.

Since Mission 1, my understanding of Cloud Computing has evolved from mainly understanding basic cloud concepts to seeing how cloud services can actually be deployed and managed. I now have a better understanding of containers, networking, storage, multi-tier architecture, and infrastructure configuration. This mission also showed me that cloud engineering requires careful planning, documentation, troubleshooting, and automation.

## References

1. Docker Documentation. **Docker Compose.**
   https://docs.docker.com/compose/

2. Docker Documentation. **Docker Compose file reference.**
   https://docs.docker.com/reference/compose-file/

3. Nextcloud Documentation. **Installation.**
   https://docs.nextcloud.com/server/latest/admin_manual/installation/

4. Docker Documentation. **Environment variables.**
   https://docs.docker.com/compose/how-tos/environment-variables/
