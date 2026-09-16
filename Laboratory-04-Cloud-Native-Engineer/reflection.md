# Mission Reflection

This activity helped me see the difference between using a Virtual Machine and using a Docker container in an actual environment. A Virtual Machine requires its own operating system, so there are more steps before it is ready to use. A Docker container is different because it shares the host operating system. Because of this, I noticed that a container can be started much faster and with a simpler setup.

Port mapping was another concept that became clearer to me during the activity. The `-p 8080:80` option connects port 8080 of the host to port 80 inside the Nginx container. This connection allowed me to access the web server through `localhost:8080`. Seeing the Nginx response in the terminal made the purpose of port mapping easier for me to understand.

I also learned that containers have a lifecycle. I could see the Nginx container while it was running, stop it, verify its status, and then remove it. When `docker rm` removes a container, data that exists only in its writable container layer is also removed. This taught me that important data should be handled properly when containers are used.

For DevOps, I think containers can make collaboration more consistent. Developers can package an application with what it needs, while the operations team can run the same container in another environment with fewer setup differences.

My GitHub portfolio is also becoming more useful as I continue these laboratory activities. It does not only show finished documents anymore. It now includes the commands I executed, screenshots of my results, and explanations of what I learned. For me, this makes my portfolio a clearer record of the cloud computing skills I am practicing.
