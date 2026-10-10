# Docker Compose Guide

## Introduction

Docker Compose is a tool used to define and manage multiple Docker containers using a YAML configuration file. In this mission, it is used to deploy Nextcloud and MariaDB together.

## 1. What Does the Services Block Do?

The `services:` block defines the containers required by the application. In the configuration file, there are two services: `database` and `app`.

The `database` service uses the `mariadb:10.6` image, while the `app` service uses the `nextcloud` image. The application service also maps port 8080 on the host to port 80 inside the container.

## 2. How Does Nextcloud Find the Database?

The environment variable `MYSQL_HOST=database` tells Nextcloud to connect to the database service named `database`. Docker Compose creates a shared network that allows the containers to communicate using their service names.

The database name, username, and password must match between the two services so that Nextcloud can connect successfully.

## 3. Difference Between Docker Run and Docker Compose Up

The `docker run` command is commonly used to create and start an individual container. When an application requires several containers, each one may need to be configured separately.

The `docker-compose up -d` command reads the Compose file and starts all the services defined in it. The `-d` option runs the containers in the background.

## 4. Important Commands

| Command | Purpose |
|---|---|
| `mkdir nextcloud-deployment` | Creates the project directory |
| `cd nextcloud-deployment` | Opens the project directory |
| `nano docker-compose.yml` | Creates or edits the Compose file |
| `cat docker-compose.yml` | Displays the configuration |
| `docker-compose up -d` | Starts the services |
| `docker-compose ps` | Checks the container status |
| `docker-compose down` | Stops and removes the containers |

If the environment uses the newer Docker Compose plugin, use `docker compose` instead of `docker-compose`.

## 5. Infrastructure as Code

Infrastructure as Code (IaC) is the practice of defining infrastructure through configuration files instead of relying only on manual commands. The Compose file defines the services, images, ports, and environment variables needed for the deployment.

This approach makes the deployment easier to repeat, manage, and share with other engineers.

## 6. Security Considerations

The passwords in the laboratory configuration are examples for testing. In real deployments, strong passwords and secure secret-management practices should be used. Sensitive credentials should not be published in a public GitHub repository.

## Conclusion

This mission demonstrated how Docker Compose can manage multiple containers using one configuration file. It also provided experience with YAML, container communication, and Infrastructure as Code.
