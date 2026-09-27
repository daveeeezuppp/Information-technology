# Cloud Storage Types Research

## Comparison of Cloud Storage Types

| Feature / Storage Type | Block Storage | File Storage | Object Storage |
| :--- | :--- | :--- | :--- |
| **Description** | Stores data in fixed-sized blocks like a raw hard drive. | Stores data in a hierarchical folder/file tree structure. | Stores data as discrete objects with metadata and a unique identifier in a flat namespace. |
| **Primary Use Case** | Databases, OS boot volumes, high-performance transactional apps. | Shared network drives, local file sharing across servers. | Storing unstructured data like images, videos, backups, and large files. |
| **Cloud Provider Example** | AWS EBS (Elastic Block Store) | AWS EFS (Elastic File System) | AWS S3 (Simple Storage Service) |

## Recommendation for Client

Object storage is the best choice for storing user-uploaded photos because it scales effortlessly to handle billions of unstructured files without performance degradation. Unlike block or file storage, object storage uses flat architecture and custom metadata, making photo retrieval fast, highly available, and far more cost-effective for web applications.
