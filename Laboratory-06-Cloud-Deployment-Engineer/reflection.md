# Mission 6 Reflection: The Cloud Deployment Engineer

During Mission 6, I learned how to deploy a private cloud storage application using Docker Compose. I learned that instead of setting up every container separately, I can define the services in one YAML configuration file and manage them together.

Writing a `docker-compose.yml` file makes a cloud engineer's job easier because all the configurations are organized in one place. The engineer can use a single command to start the application instead of manually entering many commands. It also makes the deployment easier to repeat and maintain.

I learned that indentation is important in YAML files. If I use the wrong spaces or a Tab instead of spaces, the configuration may not work correctly. Docker Compose might show an error or fail to start the services. This is why checking the format of the file is important.

Environment variables such as `MYSQL_PASSWORD`, `MYSQL_DATABASE`, and `MYSQL_USER` provide the database settings needed by the application. These variables help Nextcloud identify the database name, username, and password. I also learned that real passwords should be protected and should not be shared publicly.

Deploying Nextcloud was an interesting experience because it showed me how a web application and a database can work together. It helped me understand that cloud computing involves more than storing files online. It also requires managing the services and infrastructure that make applications work.

Since Mission 1, my understanding of cloud computing has improved. I have learned more about cloud infrastructure, services, containers, and deployment tools. This mission helped me understand the importance of automation and proper documentation. I believe these skills will be useful in my future IT projects and career. I still need more practice, but I am more confident about using Docker Compose and understanding how multiple containers work together.
