# Mission 6: The Cloud Deployment Engineer

## Mission Overview
This laboratory demonstrates how to deploy a multi-tier private cloud storage application using Docker Compose. The system consists of Nextcloud as the web application tier and MariaDB as the database tier.

## Objectives
- Understand two-tier application architecture.
- Create a Docker Compose YAML configuration.
- Deploy Nextcloud and MariaDB containers.
- Access the Nextcloud setup page through a browser.
- Document Infrastructure as Code (IaC) and deployment procedures.

## Commands Executed
```bash
mkdir nextcloud-deployment
cd nextcloud-deployment
nano docker-compose.yml
docker-compose up -d
docker-compose ps
docker-compose down
```

## Skills Learned
- Linux command-line navigation and text editing.
- Docker Compose configuration and deployment.
- Multi-container networking.
- Cloud application testing and troubleshooting.
- Markdown documentation and GitHub portfolio management.

## Evidence
Screenshots of deployment, the Nextcloud setup page, and container teardown are stored in the `screenshots/` directory.
