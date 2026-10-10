# Mission 6: The Cloud Deployment Engineer

## Mission Overview

This mission is about deploying a private cloud storage application using Docker Compose. The application uses Nextcloud as the web application and MariaDB as the database. Both services are defined in one YAML configuration file to make deployment easier and more organized.

## Objectives

- Understand two-tier architecture.
- Create a Docker Compose configuration file.
- Deploy Nextcloud and MariaDB using Docker Compose.
- Access the Nextcloud installation page through a web browser.
- Understand Infrastructure as Code (IaC).
- Document the deployment process using Markdown.

## Commands Executed

```bash
docker --version
docker-compose --version
mkdir nextcloud-deployment
cd nextcloud-deployment
nano docker-compose.yml
cat docker-compose.yml
docker-compose up -d
docker-compose ps
docker-compose down
```

## Skills Learned

I learned how to create a YAML configuration file, deploy multiple containers, check container status, and access a web application through a browser. I also learned how Docker Compose makes application deployment easier by managing multiple services using one configuration file.

## Screenshots

The screenshots are stored in the `screenshots/` folder.

- `compose-deployment.png` - Successful container deployment.
- `nextcloud-web.png` - Nextcloud installation page.
- `compose-teardown.png` - Container shutdown process.

## Conclusion

This mission helped me understand how Nextcloud and MariaDB work together in a multi-container environment. It also improved my knowledge of Docker Compose and Infrastructure as Code.
