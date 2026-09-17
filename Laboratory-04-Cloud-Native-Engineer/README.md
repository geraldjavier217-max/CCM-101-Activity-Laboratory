# Laboratory 04 — The Cloud-Native Engineer

## Mission Overview

This laboratory activity introduces containerization and the basic concepts of cloud-native engineering. The activity compares Virtual Machines and containers and demonstrates how Docker can be used to deploy an Nginx web server quickly and efficiently.

## Objectives

* Differentiate Virtual Machines from containers.
* Access a Docker-enabled cloud environment using KillerCoda.
* Execute fundamental Docker CLI commands.
* Pull and run an Nginx container.
* Map a host port to a container port.
* Manage the lifecycle of a Docker container.
* Document Docker operations using Markdown.
* Maintain an organized GitHub Cloud Computing Portfolio.

## Docker Commands Executed

### Docker Verification

```bash
docker --version
docker info
docker ps
```

### Nginx Deployment

```bash
docker pull nginx
docker run -d --name nginx-server -p 8080:80 nginx
docker ps
curl http://localhost:8080
```

### Container Lifecycle

```bash
docker stop nginx-server
docker ps
docker ps -a
docker rm nginx-server
docker ps -a
```

## Skills Learned

Through this laboratory activity, I learned how to verify Docker, download container images, create and run containers, map network ports, test a web server, and manage the container lifecycle. I also practiced documenting technical procedures using Markdown and organizing evidence in a GitHub repository.

## Challenges Encountered

One challenge was understanding the difference between a Docker image and a running container. Another challenge was understanding port mapping and how port 8080 on the host connects to port 80 inside the Nginx container. Working through the commands and checking the terminal output helped me understand how Docker manages applications.

## Screenshots

* `screenshots/docker-version.png`
* `screenshots/nginx-running.png`
* `screenshots/container-lifecycle.png`

