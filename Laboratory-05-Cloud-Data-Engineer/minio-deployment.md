# MinIO Deployment

## Deployment Process

For this laboratory activity, I deployed MinIO as an object storage server using Docker in the KillerCoda Ubuntu Playground. I used Docker to download the MinIO image, create the container, configure the login credentials, and make the web console accessible.

## Docker Command Used

The exact Docker command I used to deploy the MinIO server was:

```bash
docker run -d -p 9000:9000 -p 9001:9001 --name minio-server -e "MINIO_ROOT_USER=cloudadmin" -e "MINIO_ROOT_PASSWORD=CloudNova2026!" quay.io/minio/minio server /data --console-address ":9001"
