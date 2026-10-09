# Mission 6: The Cloud Deployment Engineer

## Mission Overview

This mission demonstrates how to deploy a multi-tier private cloud storage application using Docker Compose. The deployment consists of Nextcloud as the web application and MariaDB as the database.

## Objectives

* Understand two-tier architecture.
* Create a Docker Compose YAML configuration file.
* Deploy Nextcloud and MariaDB containers.
* Access the Nextcloud web interface through port 8080.
* Document Infrastructure as Code principles.
* Maintain a professional GitHub cloud computing portfolio.

## Commands Executed

```bash
mkdir nextcloud-deployment
cd nextcloud-deployment
nano docker-compose.yml
docker-compose up -d
docker-compose ps
docker-compose logs app
docker-compose down
```

## Skills Learned

* Understanding multi-tier application architecture.
* Writing YAML configuration files.
* Using Docker Compose to manage multiple containers.
* Connecting an application container to a database container.
* Accessing a containerized web application.
* Documenting deployment procedures using Markdown.
* Applying Infrastructure as Code principles.

## Screenshots

The `screenshots/` folder contains evidence of the deployment, Nextcloud web interface, and container teardown.

## Conclusion

This mission provided practical experience deploying a multi-container cloud application with Docker Compose. It demonstrated how Infrastructure as Code makes deployment easier to repeat, manage, and document.
