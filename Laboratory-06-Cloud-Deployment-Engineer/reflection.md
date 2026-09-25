# Laboratory 06 Reflection

Writing a docker-compose.yml file makes a cloud engineer's job easier because it allows multiple services to be configured and deployed using one file. Instead of manually typing commands for each container, Docker Compose can start the application and database together using docker-compose up -d. It also makes the deployment easier to repeat because the configuration is already written in the YAML file.

I also learned that YAML is sensitive to indentation. If I use a Tab instead of spaces or place the indentation incorrectly, the YAML file may produce an error and Docker Compose may not be able to read the configuration properly. This showed me that careful formatting is important when writing Infrastructure as Code.

We used environment variables such as MYSQL_PASSWORD, MYSQL_DATABASE, and MYSQL_USER because they provide the configuration values needed by the containers. These variables allow the Nextcloud application and MariaDB database to use the required database settings and communicate with each other correctly.

It was interesting to see how a fully functional enterprise cloud storage system like Nextcloud could be deployed in only a few minutes. The activity helped me understand that cloud deployment can be made faster and more organized when automation tools such as Docker Compose are used. Seeing the Nextcloud setup page in the browser also helped me connect the commands I entered in the terminal to an actual working application.

Since Mission 1, my understanding of Cloud Computing has changed because I now have a better understanding of how cloud environments are built, managed, and documented. I learned that cloud computing is not only about accessing services through the internet, but also involves Linux, containers, networking, storage, automation, and Infrastructure as Code. This laboratory helped me see how these concepts can work together to create and manage a cloud application.
