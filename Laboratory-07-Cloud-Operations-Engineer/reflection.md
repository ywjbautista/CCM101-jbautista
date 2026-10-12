
# Laboratory 07 Reflection

Checking the host server's resources is important even when containers appear to be running properly. Containers still depend on the host's available CPU, memory, and disk space. If these resources become limited, the application may slow down or stop responding even when the container has started successfully.

The `docker logs` command helps investigate a user's login problem by showing requests and errors recorded by the application. An engineer can review the available log entries to identify failed requests and determine what to investigate next. Logs may not explain every issue, but they provide useful evidence for troubleshooting.

Logs and metrics serve different purposes. Logs record application events and requests, including unsuccessful requests such as HTTP 404 errors. Metrics provide numerical measurements, such as CPU percentage, memory consumption, and network activity. Reviewing both gives a more complete picture of application health.

Large companies can monitor thousands of containers using centralized monitoring platforms. Prometheus can collect metrics, while Grafana can display information through dashboards. These tools help teams recognize unusual patterns and monitor many containers more efficiently than checking each one manually.

This activity improved my ability to troubleshoot Linux environments by giving me practice with commands for checking system resources, deploying a web server, generating HTTP requests, and inspecting Docker logs and metrics. I learned that a running container does not automatically prove that an application is healthy. Engineers need to examine evidence, monitor resource usage, and investigate errors before deciding whether a service is operating correctly.
