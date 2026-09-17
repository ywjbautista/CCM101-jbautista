# Understanding Cloud Storage Types

Cloud storage can be organized in different ways depending on how the data will be used. The three common types are Block Storage, File Storage, and Object Storage.

| Storage Type | Description | Primary Use Case | Cloud Provider Example |
|---|---|---|---|
| Block Storage | Data is divided into separate blocks that can be accessed and managed by the system individually. | Best for workloads that need fast access, such as virtual machine disks and databases. | AWS EBS |
| File Storage | Data is arranged using familiar files and folders that can be shared through a network. | Best for shared documents and applications where several users or systems need access to the same files. | AWS EFS |
| Object Storage | Data is stored as individual objects together with information about each object instead of using a traditional folder or disk structure. | Best for large amounts of unstructured data such as photos, videos, backups, and media files. | AWS S3 |

## Recommendation for the Client

For a photo-sharing application, Object Storage fits the client's needs because uploaded images can be stored as separate objects and managed at a large scale. It is designed for large amounts of unstructured data, making it more suitable for millions of user-uploaded photos than storing everything directly inside the web server.
