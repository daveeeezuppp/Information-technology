# Mission 6 Reflection

In Mission 6, I learned how to deploy a multi-container application using Docker Compose. Before this activity, I understood that Docker could run applications inside containers, but I did not fully understand how multiple containers could work together. Using Nextcloud and MariaDB helped me understand how a web application communicates with a database.

Writing a `docker-compose.yml` file makes a cloud engineer's job easier because the configuration for the services is written in one place. Instead of running several long commands manually, an engineer can use one command to start the entire application. This approach reduces repetitive work, keeps the configuration organized, and makes deployments easier to repeat.

I also learned that indentation is important in YAML files. If I use incorrect spacing or a tab where spaces are expected, Docker Compose may report an error or interpret the configuration incorrectly. This taught me to check the structure of my code carefully before deploying the application.

Environment variables such as `MYSQL_PASSWORD`, `MYSQL_DATABASE`, and `MYSQL_USER` provide the configuration required by the database and application. They allow the services to use matching database credentials and settings. I also learned that `MYSQL_HOST=database` allows Nextcloud to locate the MariaDB service through its Compose service name.

Deploying Nextcloud was an interesting experience because it showed me how a private cloud storage application can be prepared in a short time using existing container images. I understood that a successful deployment still requires checking container status, reviewing logs, and testing access through a browser.

Since Mission 1, my understanding of cloud computing has grown from learning basic cloud concepts to applying practical deployment skills. I now better understand how containers, networking, databases, and configuration files work together. This mission also taught me that documentation, troubleshooting, and careful configuration are important responsibilities for a cloud engineer.

Overall, Mission 6 helped me appreciate Infrastructure as Code and gave me more confidence in managing containerized applications. I want to continue improving my Docker skills and learn how to deploy applications securely in a real cloud environment.
