# Mission 6 Reflection: The Cloud Deployment Engineer

This laboratory activity helped me understand how Docker Compose makes cloud deployment easier and more organized. Instead of manually creating and configuring each container, I learned that I can write a `docker-compose.yml` file that describes the services and their settings. By using one command, I can start multiple containers together. This saves time, reduces repetitive work, and makes the deployment process easier to repeat.

I also learned that YAML indentation is very important. If I accidentally use a tab instead of spaces or place a setting at the wrong indentation level, the configuration may produce an error or fail to work as expected. This taught me to check the structure of my file carefully before deploying an application.

Environment variables, such as `MYSQL_PASSWORD` and `MYSQL_DATABASE`, provide configuration values that the application and database need to communicate. They help organize settings in the Compose file. However, I also learned that passwords written directly in a configuration file should only be used for demonstrations, not for real production systems. In an actual deployment, secrets should be managed more securely.

Deploying Nextcloud was a valuable experience because it showed me how a private cloud storage application can run using two connected containers. Seeing the setup page in my browser helped me connect the commands in the terminal with the actual application users would access. I also learned the importance of checking container status, reviewing logs when problems occur, and shutting down services properly.

Since Mission 1, my understanding of cloud computing has grown from learning basic concepts and services to understanding how different technologies work together. I now see that cloud engineering involves more than starting a server. It requires planning, configuration, testing, documentation, and security. This mission introduced me to Infrastructure as Code and helped me appreciate how automation makes deployments more consistent and manageable. I can apply these skills to future cloud projects and improve my technical portfolio.
