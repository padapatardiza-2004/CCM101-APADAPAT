# Storage Types Research

## Comparison of Cloud Storage Types

| Storage Type | Description | Primary Use Case | Cloud Provider Example |
|---|---|---|---|
| Block Storage | Stores data in blocks that can be attached to a virtual machine and used like a disk. | Operating systems, databases, and applications requiring fast disk access. | AWS EBS |
| File Storage | Stores data as files in folders and directories and can be shared over a network. | Shared documents, media files, and applications requiring a shared file system. | AWS EFS |
| Object Storage | Stores data as individual objects with metadata and unique identifiers inside buckets. | Images, videos, backups, documents, and other unstructured data. | Amazon S3 |

## Why Object Storage Is Suitable for Millions of User-Uploaded Images

Object Storage is suitable for millions of user-uploaded images because it is designed to handle large amounts of unstructured data. Each image can be stored as an object inside a bucket and accessed through APIs, making it practical for applications that need to store and retrieve many images.
