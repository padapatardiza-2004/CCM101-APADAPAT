## Mission Overview

This mission focused on deploying a private cloud storage application using a multi-tier container architecture. Nextcloud was used as the web application while MariaDB provided the database service, with Docker Compose used to manage both containers.

## Objectives

* Explain the purpose of a two-tier application architecture.
* Understand the structure and purpose of a Docker Compose YAML file.
* Use `nano` through the Linux command line.
* Deploy a multi-container application with Docker Compose.
* Understand basic Infrastructure as Code concepts.
* Document the deployment using Markdown.
* Add the completed work to the Cloud Computing GitHub portfolio.

## Commands Executed

The main commands used during the activity were:

```bash
mkdir nextcloud-deployment
cd nextcloud-deployment
nano docker-compose.yml
docker-compose up -d
docker-compose ps
docker-compose down
```

## Skills Learned

This activity helped me practice working with Docker Compose, YAML configuration, Linux command-line tools, container communication, environment variables, multi-container deployment, and Markdown documentation. I also gained experience connecting a containerized web application with a separate database service.
