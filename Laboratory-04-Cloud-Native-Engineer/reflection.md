
---

# CHECKPOINT 7 — Reflection

Create:

**`reflection.md`**

Use this **250–350 word reflection**:

```markdown
# Mission 4 Reflection

This laboratory activity helped me understand the difference between traditional Virtual Machines and Docker containers. A Docker container can start much faster than a Virtual Machine because a container does not need to boot a complete operating system. A Virtual Machine needs a guest operating system and its system services before an application can run, which requires more time and resources. In comparison, a container shares the host operating system kernel and only needs to start the application and its required dependencies.

The port mapping `-p 8080:80` is necessary because the Nginx web server is running on port 80 inside the container, while port 8080 is used on the host machine. The mapping connects the host's port 8080 to the container's port 80. This allows users or applications on the host to access the Nginx web server by using `http://localhost:8080`.

When the `docker rm` command is used, the container itself is permanently removed after it has been stopped. Data stored only inside the container's writable layer is also removed. This is why important data should be stored using persistent storage such as Docker volumes when the data needs to remain available after a container is deleted.

Containerization also changes how developers and IT operations teams work together. Developers can package an application and its dependencies into a container, while operations teams can deploy the same container in different environments. This improves consistency between development, testing, and production and supports the DevOps approach.

My GitHub portfolio is also evolving as I add more practical cloud computing activities. Instead of only documenting concepts, I am now including actual commands, deployment procedures, screenshots, and technical reflections. This laboratory adds Docker and cloud-native engineering to my portfolio and provides evidence of my practical skills.
