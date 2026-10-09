# MinIO Deployment Documentation

## 1. Deployment Overview

MinIO is an object storage server that allows users to store and manage files such as images, videos, and documents. In this laboratory, I deployed MinIO using Docker.

## 2. Docker Command Used

The Docker command used to deploy the MinIO server was:

```bash
docker run -d \
  --name minio-server \
  -p 9000:9000 \
  -p 9001:9001 \
  -e "MINIO_ROOT_USER=minioadmin" \
  -e "MINIO_ROOT_PASSWORD=minioadmin123" \
  quay.io/minio/aistor/minio:RELEASE.2026-03-26T21-24-40Z server /data
```

Note: Use the exact command and image that worked in your environment. The command above is an example; your actual image or required arguments may differ.

## 3. Web Console Port

The MinIO web console uses port **9001**.

The MinIO API uses port **9000**.

## 4. Bucket Created

Bucket name: `student-photos`

The bucket is used to organize and store objects such as images, documents, and other files.

Replace `student-photos` with the actual bucket name you created.

## 5. Environment Variables

The `-e` flags define environment variables inside the Docker container.

* `MINIO_ROOT_USER` sets the administrator username.
* `MINIO_ROOT_PASSWORD` sets the administrator password.

These variables configure administrator credentials for the MinIO server. For a real deployment, use strong credentials and do not publish passwords in documentation.

## 6. Deployment Result

Docker was used to run the MinIO storage server in a container. Ports 9000 and 9001 were mapped so that the storage API and web console could be accessed through the host environment.

