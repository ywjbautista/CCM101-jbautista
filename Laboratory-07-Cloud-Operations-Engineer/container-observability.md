# Container Observability Report

## Application Logs

### HTTP 404 Error

`172.17.0.1 - - [12/Oct/2026:01:26:30 +0000] "GET /hidden-admin-page HTTP/1.1" 404 153 "-" "curl/8.5.0" "-"`

Application logs help engineers identify failed requests and investigate application problems. In this activity, the logs showed three successful HTTP 200 requests and one HTTP 404 request for `/hidden-admin-page`. This information helps engineers identify which request failed and investigate the cause.

## Container Metrics

- Memory Usage: 2.738MiB
- CPU Percentage: 0.00%

The Docker stats output showed that the `client-website` container was using 2.738MiB of memory and 0.00% CPU at the time the screenshot was taken.
