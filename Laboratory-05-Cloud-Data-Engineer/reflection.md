# Mission Reflection

This activity helped me understand why choosing the correct storage type is important in cloud computing. For an application that stores millions of photos, Object Storage is more suitable than using a traditional block storage hard drive. Photos are unstructured data, and Object Storage is designed to handle large collections of individual objects.

Docker made the MinIO deployment easier because most of the setup was included in one command. I could define the ports, credentials, container name, and storage server without manually installing every part. I also encountered a problem when the original MinIO image could not be pulled. After checking the problem, I was able to use an available MinIO image while keeping the required configuration.

Creating the `client-photos` bucket helped me understand what a bucket actually does. I now understand it as a container where objects can be stored and organized. Uploading my sample file made the idea easier to understand because I could actually see the object inside the bucket.

For large companies, keeping important data on only one physical server would be risky. They can maintain redundant copies of data across multiple servers or locations. Backup and replication can also help keep the data available if one physical machine fails.

I am becoming more comfortable using the Linux command line compared with my earlier laboratory activities. I still check commands carefully before entering them, but I can understand more of the terminal output now. The MinIO image problem also taught me that reading error messages is important when something does not work as expected.
