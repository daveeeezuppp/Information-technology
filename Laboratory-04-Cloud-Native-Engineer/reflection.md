# Mission 4 Reflection

## 1. How does the boot time and setup process of a Docker container compare to installing an operating system on a Virtual Machine?

A Docker container starts much faster than a Virtual Machine because it does not need to install or boot a complete operating system. A container shares the host operating system kernel and only starts the application and its required dependencies. In contrast, a Virtual Machine needs a complete guest operating system, which requires more time, storage, and system resources.

## 2. Why is port mapping (-p 8080:80) necessary when running a web server inside a container?

Port mapping `-p 8080:80` connects port 8080 on the host machine to port 80 inside the Docker container. Nginx runs on port 80 inside the container, so the mapping allows the host to access the web server using `http://localhost:8080`. Without port mapping, the web server would not be directly accessible through the host's port 8080.

## 3. What happens to the data inside a container when you use the docker rm command?

The `docker rm` command permanently removes a stopped container. Any data stored only inside the container's writable layer is also removed. Important data should therefore be stored using persistent storage such as Docker volumes if it needs to remain after the container is deleted.

## 4. How do you think containerization changes the way software developers and IT operations teams work together (DevOps)?

Containerization makes collaboration between developers and IT operations easier because developers can package an application together with its dependencies inside a container. IT operations teams can then use the same container in development, testing, and production environments. This creates more consistent deployments and reduces problems caused by differences between environments.

## 5. How is your GitHub portfolio evolving?

My GitHub portfolio is evolving from basic documentation into a more practical collection of technical projects and laboratory activities. In this activity, I added Docker commands, container deployment, Nginx testing, container lifecycle management, screenshots, and technical documentation. This shows my growing knowledge of cloud computing, Docker, and cloud-native engineering.
