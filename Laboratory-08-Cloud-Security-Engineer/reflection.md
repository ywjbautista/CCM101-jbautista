# Reflection — The Cloud Security Engineer

A host-based firewall protects an individual server by controlling the network traffic that can reach it. Even if the physical network perimeter is breached, the server can still reject incoming connections that are not explicitly permitted. This provides another layer of defense and helps reduce the risk of unauthorized access.

Managing open network ports is important because each exposed service creates another possible entry point for attackers. If a server only needs SSH for administration and port 8080 for its web application, unnecessary ports should remain closed. Limiting access to required services reduces the server's attack surface.

Leaving a database port such as MySQL's 3306 open to the public internet is dangerous because attackers may attempt unauthorized logins or exploit vulnerabilities. A database can contain sensitive information, so access should be limited to trusted applications and administrators. Strong authentication and other security controls are also necessary.

This mission helped me understand that deploying an application is not enough to make a server secure. Its network access must also be reviewed and controlled. I learned that configuring firewall rules, checking their status, and testing the application after changes are important steps in protecting a server.

My GitHub portfolio records my progress through the cloud computing missions. The earlier activities introduced cloud concepts and infrastructure, while later missions provided practice in deployment, monitoring, and security. Organizing the work with Markdown files and screenshots also helps me review and explain what I have done. Overall, this mission taught me that security is an ongoing responsibility and that reliable cloud operations require careful configuration, testing, and documentation.
