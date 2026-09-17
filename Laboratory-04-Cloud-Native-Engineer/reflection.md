# Mission Reflection

This laboratory activity helped me understand how containerization can make application deployment faster and more efficient. When using a Virtual Machine, a complete operating system needs to be installed and started before an application can run. This process can require more time and system resources. In comparison, a Docker container uses the host operating system's kernel and only includes the components needed by the application. Because of this, containers can start much faster and generally require fewer resources than full Virtual Machines.

The port mapping `-p 8080:80` is necessary because the Nginx web server is running inside the container on port 80, while port 8080 is used to access it from the host environment. The mapping connects the host's port 8080 to the container's port 80. When I accessed `http://localhost:8080`, Docker forwarded the request to Nginx inside the container. Seeing the "Welcome to nginx!" response confirmed that the port mapping was working correctly.

When `docker rm` is used, the specified container is removed from Docker. Any data stored only inside the container's writable layer is removed with the container, while the Docker image remains available. This showed me why applications that need persistent data should use appropriate storage such as Docker volumes.

Containerization can also improve collaboration between developers and IT operations teams. Developers can package an application and its dependencies into a consistent container, while operations teams can deploy that container in different environments. This supports DevOps practices by making deployment and application management more consistent.

Finally, my GitHub portfolio is evolving from simply containing individual laboratory outputs into a more organized record of my cloud computing skills. Each laboratory adds new technical knowledge and practical experience that I can demonstrate through documented commands, screenshots, and reflections.

