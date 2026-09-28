# Types of Cloud Storage

| Storage Type       | Description                                                                                                                      | Primary Use Case                                                                                  | Cloud Provider Example             |
| ------------------ | -------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------- | ---------------------------------- |
| **Block Storage**  | Stores data in fixed-size blocks that can be accessed individually. The storage appears to a computer like a disk drive.         | Operating system disks, databases, and applications that require fast and consistent disk access. | AWS Elastic Block Store (EBS)      |
| **File Storage**   | Stores data as files organized into folders and directories. Multiple systems can access the same file structure over a network. | Shared files, documents, team folders, and applications that require a traditional file system.   | Amazon Elastic File System (EFS)   |
| **Object Storage** | Stores data as objects together with metadata and a unique identifier inside containers called buckets.                          | Large amounts of unstructured data such as images, videos, backups, and documents.                | Amazon Simple Storage Service (S3) |

## Why Object Storage Is Suitable for the Client

Object Storage is suitable for the photo-sharing application because it is designed to handle large amounts of unstructured data such as user-uploaded images. It can organize files using buckets and object metadata while allowing applications to access the stored data through web-based APIs.

