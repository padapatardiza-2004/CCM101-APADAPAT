# Mission Reflection

This laboratory helped me understand how Docker containers are different from Virtual Machines. When using a Virtual Machine, a complete operating system needs to be installed and started, so it usually takes more time and uses more resources. With Docker, I was able to run Nginx in a container without installing another complete operating system. I found containers more convenient for this kind of web application because they are lightweight and can start faster.

The `-p 8080:80` part of the Docker command is used for port mapping. Port 8080 is the port I used on the host, while port 80 is the port used by Nginx inside the container. This allowed me to access the Nginx web server through `http://localhost:8080`. Without the port mapping, I would not be able to access the Nginx service through that host port.

When I used `docker rm nginx-server`, the container was removed. Any data that was stored only inside the container's writable layer would not remain after the container was removed. This helped me understand why persistent data should be stored using volumes when it needs to be kept even after deleting a container.

Containerization can also improve teamwork between developers and IT operations. Developers can package an application with the environment it needs, while the IT team can run the same container without having to manually set up everything again. This supports the DevOps approach because development and deployment can become more consistent.

My GitHub portfolio is also improving as I complete more laboratory activities. This laboratory added Docker, containerization, commands, documentation, and screenshots to my previous cloud computing work. It shows my progress and the new skills I learned from the activity.

