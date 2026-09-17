# My MinIO Object Storage Deployment

## Deployment Process

For this activity, I used Docker to create a working MinIO object storage server. The MinIO image in the activity could not be pulled in my current environment, so I used the available image from `quay.io` while keeping the required ports, credentials, and server configuration.

## Docker Command Used

`docker run -d -p 9000:9000 -p 9001:9001 --name minio-server -e "MINIO_ROOT_USER=cloudadmin" -e "MINIO_ROOT_PASSWORD=CloudNova2026!" quay.io/minio/minio server /data --console-address ":9001"`

The command created a container named `minio-server`. Port `9000` was used for the MinIO API, while port `9001` allowed me to access the web console.

## Web Console Access

I accessed the MinIO web console through port `9001`. The browser interface allowed me to manage the storage environment after deploying the server from the terminal.

## Bucket Created

I created a bucket named `client-photos` and uploaded a sample file inside it. This confirmed that the object storage environment was working.

## Environment Variables

The `-e` flags passed environment variables into the container. `MINIO_ROOT_USER` defined the root username, while `MINIO_ROOT_PASSWORD` defined the password used to access MinIO.
