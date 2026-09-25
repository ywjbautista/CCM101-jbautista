# Laboratory 06 Reflection

## 1. What did you learn about multi-tier applications?

I learned that a multi-tier application separates different parts of the system into different services. In this laboratory, Nextcloud served as the application tier while MariaDB served as the database tier.

## 2. Why is Docker Compose useful for multi-container applications?

Docker Compose is useful because it allows multiple containers to be configured and managed together using one configuration file. It makes starting and stopping the application easier.

## 3. What role does the database container play?

The database container stores and manages the data needed by the application. In this laboratory, MariaDB provided the database service for Nextcloud.

## 4. What challenges did you encounter?

One challenge I encountered was making sure that the Docker Compose commands were executed in the correct directory. I also learned that the application and database containers must both be running for the multi-tier application to work properly.

## 5. How could this architecture be improved?

The architecture could be improved by adding more security, proper data backups, and persistent storage. These improvements would help protect the application and its data in a real cloud deployment.
