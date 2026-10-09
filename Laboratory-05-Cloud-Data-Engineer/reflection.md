# Checkpoint 6 – Mission Reflection

### 1. Why is object storage better suited for storing millions of photos compared to a traditional block storage hard drive?

Object storage is better for storing millions of photos because it can manage a large amount of unstructured data efficiently. Each photo is stored as an object with its own unique identifier and metadata. It is easier to organize, search, and access photos without managing individual disk blocks. Object storage can also scale when the number of photos increases.

### 2. How did using Docker make it easier to deploy the MinIO storage server?

Docker made deploying the MinIO storage server easier because it allowed me to run MinIO inside a container. I did not need to install and configure every dependency manually. Docker also made it easier to manage the server and expose its ports. This helped me understand how containers simplify application deployment.

### 3. What is a "bucket" in the context of cloud storage?

A bucket is a container used to store and organize objects in a cloud storage system. It can contain files such as photos, videos, documents, and other data. For example, I can create a bucket named `student-photos` to store student pictures. Buckets help organize data and make it easier to manage.

### 4. How do you think large enterprise companies ensure their object storage data is not lost if the physical server crashes?

Large enterprise companies protect their data by keeping multiple copies across different disks, servers, or locations. They may use replication and erasure coding to recover data when hardware fails. They also perform regular backups and monitor their storage systems. These methods help ensure that files remain available even if a physical server crashes.

### 5. How is your confidence in navigating the Linux command line growing?

My confidence in using the Linux command line is growing because I am learning how to execute commands and manage containers. I became more familiar with navigating directories, running Docker commands, and checking server logs. Although I still need more practice, I feel more comfortable troubleshooting errors and completing tasks using the terminal.

