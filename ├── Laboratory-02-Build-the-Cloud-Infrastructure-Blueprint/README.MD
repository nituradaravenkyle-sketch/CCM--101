# Mission 5: The Cloud Data Engineer

## Mission Overview

This laboratory activity focused on understanding cloud storage and deploying an S3-compatible object storage server using MinIO. Using the KillerCoda Playground, I deployed MinIO with Docker, accessed its web console, created a storage bucket, and uploaded a sample file. The activity also helped me understand the differences between Block Storage, File Storage, and Object Storage.

## Objectives

- Explain the differences between Block Storage, File Storage, and Object Storage.
- Deploy an S3-compatible Object Storage server using MinIO.
- Use Docker to run a cloud storage server.
- Access the MinIO Web Console using port forwarding.
- Create a storage bucket and upload an object.
- Document cloud storage operations using Markdown.
- Practice professional technical documentation using GitHub.

## Cloud Storage Components

### Block Storage

Block Storage stores data in fixed-size blocks that can be accessed individually. It is commonly used for operating systems, databases, and applications that require fast disk access.

### File Storage

File Storage organizes data into files and folders through a shared file system. It is useful for shared documents, file systems, and applications that need access to shared files.

### Object Storage

Object Storage stores data as objects together with metadata and a unique identifier. It is commonly used for images, videos, backups, documents, and other types of unstructured data.

For the client's photo-sharing application, Object Storage is the best choice because it can store large amounts of user-uploaded images and can scale as the number of files increases.

## Tools Used

- KillerCoda Playground
- Ubuntu Linux
- Docker
- MinIO
- GitHub
- Web browser
- Markdown

## Docker Deployment

The MinIO server was deployed using Docker with the following command:

```bash
docker run -d -p 9000:9000 -p 9001:9001 --name minio-server -e "MINIO_ROOT_USER=cloudadmin" -e "MINIO_ROOT_PASSWORD=CloudNova2026!" minio/minio server /data --console-address ":9001"
