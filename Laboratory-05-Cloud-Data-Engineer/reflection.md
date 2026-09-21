## Reflection

Object storage is useful for storing millions of photos because it is designed to handle large amounts of unstructured data. Unlike a traditional block storage hard drive, photos can be stored as individual objects inside buckets together with their metadata. This makes it easier for applications to organize, access, and manage a very large collection of files.

Docker made deploying MinIO easier because MinIO could be started as a container without manually installing and configuring the complete application environment. The Docker command allowed the image, ports, administrator credentials, and other settings to be configured in one command. This made the deployment process faster and more organized.

A bucket is a storage container used to organize objects in an object storage system. In this activity, the bucket named client-photos was created to store the uploaded sample file. It helped demonstrate how files can be organized within an object storage service.

Enterprises can reduce the risk of object storage data loss by using redundancy, replication, backups, and multiple storage locations. These methods provide additional copies of data so that information can remain available even if a physical server or storage device becomes unavailable.

This activity also helped me become more comfortable with Linux command-line tools. I practiced commands such as docker pull, docker run, and docker ps, and learned how they can be used to deploy and verify a cloud service. I also became more familiar with checking command output and troubleshooting when something does not work as expected. Overall, the activity gave me more confidence in using Linux and Docker for cloud computing tasks.
