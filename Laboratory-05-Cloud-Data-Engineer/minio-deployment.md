# MinIO Deployment Documentation

## Deployment Overview

For this laboratory activity, MinIO was deployed on an Ubuntu environment using Docker. MinIO was used as an S3-compatible object storage service.

## Docker Command Used

The exact Docker command used to deploy the server was:

```bash
docker run -d -p 9000:9000 -p 9001:9001 --name minio-server -e "MINIO_ROOT_USER=cloudadmin" -e "MINIO_ROOT_PASSWORD=CloudNova2026!" quay.io/minio/minio server /data --console-address ":9001"
