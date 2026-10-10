# Multi-Tier Architecture

## What is a Two-Tier Architecture?

A two-tier architecture is a system design that separates an application into two main parts: the web/application tier and the database tier. These two parts communicate with each other to provide services to users. In this mission, Nextcloud is the web application, while MariaDB is the database.

## 1. The Web/Application Tier

The web/application tier handles user requests and displays the application's interface through a web browser. In this mission, Nextcloud allows users to access the private cloud storage application. It also communicates with the database to retrieve and store information.

## 2. The Database Tier

The database tier stores and manages the information needed by the application. MariaDB is used to store user account information, file metadata, and other application records.

## 3. Why Separate Them?

Separating the web application and database into two containers makes the system easier to manage, maintain, and troubleshoot. Each container has its own responsibility, and the services can be updated or scaled more independently. However, proper security and configuration are still necessary.

## Architecture Components

- Web/Application Tier: Nextcloud
- Database Tier: MariaDB
- Deployment Tool: Docker Compose
- Application Port: 8080
- Database Host: database

## How the Architecture Works

Users access Nextcloud through a web browser using port 8080. Nextcloud processes their requests and communicates with MariaDB when it needs database information. Docker Compose manages the services and allows them to communicate through a shared network.

## Conclusion

This two-tier architecture demonstrates how a web application and a database can run in separate containers while working together as one application.
