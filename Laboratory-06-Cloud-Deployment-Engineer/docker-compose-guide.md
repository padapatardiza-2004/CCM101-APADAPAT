# Docker Compose Guide

## Purpose of the `services:` Block

The `services:` block describes the separate components that make up the application. In this configuration, there are two services: `database`, which uses MariaDB, and `app`, which uses the Nextcloud image.

## How Nextcloud Finds the Database

The connection between Nextcloud and MariaDB is specified through the environment variables in the `app` service. In particular, `MYSQL_HOST=database` tells the Nextcloud container to use the service named `database` as its database host. Docker Compose allows the containers in the same application to communicate using these service names.

## Difference Between `docker run` and `docker-compose up -d`

The `docker run` command can be used to create and start a Docker container by providing its settings directly through the command line. `docker-compose up -d`, however, reads the configuration from the `docker-compose.yml` file and uses it to start the services defined in the file. This is useful when an application requires multiple containers that must work together, while the `-d` option allows them to run in the background.
