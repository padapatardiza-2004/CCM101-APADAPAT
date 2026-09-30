

## Reflection

Creating the `docker-compose.yml` file showed me how a cloud deployment can be organized in a single configuration. Instead of entering separate commands for every part of the application, the required services and their settings were written in one file. This makes the deployment process more repeatable because the same configuration can be used again when the application needs to be deployed.

One important lesson I learned was the effect of YAML formatting. YAML depends on proper spacing and indentation to understand the relationship between different settings. If the indentation is incorrect, such as using a Tab where spaces are expected, Docker Compose may fail to interpret the configuration correctly. This means that even a small formatting mistake can prevent the application from starting properly.

Environment variables also play an important role in the deployment. Values such as `MYSQL_PASSWORD`, `MYSQL_DATABASE`, and `MYSQL_USER` provide the database configuration needed by the services. The `MYSQL_HOST` value connects the Nextcloud application to the database service by identifying it as `database`.

Seeing the Nextcloud page through the browser made the activity more understandable because I could see the result of the container deployment instead of only working with terminal commands. It showed me how several components can be combined to provide an actual cloud-based application.

My understanding of Cloud Computing has changed since Mission 1. I started with the basic idea of cloud services and infrastructure, but this mission helped me understand how containers, application services, databases, networking, and configuration files can work together. I also learned that automation and proper infrastructure configuration can make deployment more organized and repeatable.
