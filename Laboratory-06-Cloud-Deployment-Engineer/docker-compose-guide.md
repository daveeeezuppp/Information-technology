# Docker Compose Guide

## What Does the `services:` Block Do?

The `services:` block defines the containers that make up the application. In this deployment, the `database` service uses MariaDB, while the `app` service uses Nextcloud. Docker Compose reads these definitions and manages the services together.

## How Does Nextcloud Find MariaDB?

The Nextcloud application uses the `MYSQL_HOST` environment variable, which is set to `database`. This matches the database service name in the Compose file. Docker Compose creates a network for the application, allowing Nextcloud to communicate with MariaDB using that service name.

## Docker Run vs. Docker Compose

The `docker run` command starts an individual container and usually requires its configuration to be supplied through command-line options. Docker Compose reads a YAML configuration file and manages multiple related services together.

The command `docker-compose up -d` creates and starts the services in the background. The `-d` option means detached mode, allowing the terminal to be used for other commands while the containers run.

## Environment Variables

Environment variables configure the database and application. For example, `MYSQL_DATABASE` specifies the database name, `MYSQL_USER` specifies the database username, and `MYSQL_PASSWORD` supplies the database user's password. The values used by Nextcloud must match the database configuration.

## Persistent Volumes

The `db_data` volume stores MariaDB data, and `nextcloud_data` stores Nextcloud application data. Named volumes help preserve data when containers are stopped or removed, provided the volumes themselves are not deleted.
ø

