
# Mission Reflection

This laboratory helped me understand why object storage is commonly used for applications that handle large amounts of unstructured data. Compared with traditional block storage, object storage is designed to manage individual objects such as images, videos, documents, and backups. For a photo-sharing application, this makes it practical to store millions of photos without placing all the data directly inside the web server. Object storage can also provide scalable access as the amount of uploaded data increases.

Docker made deploying MinIO easier because I did not have to manually install and configure every component of the storage server. With one Docker command, I was able to download the MinIO image, create a container, configure the administrator credentials, and expose the required ports. This showed me how containers can make deployment faster and more consistent.

I also learned that a bucket is a logical container used to organize objects in object storage. In this activity, I created a bucket called `client-photos` and uploaded a test file into it. This helped me understand how applications can separate and organize their stored data.

Large enterprise companies can protect object storage data from physical server failures through techniques such as redundancy, replication, backups, and distributing data across multiple systems or locations. These methods help ensure that data remains available even when individual hardware components fail.

My confidence with the Linux command line is also growing. At first, Docker commands and Linux commands seemed difficult to remember, but using commands such as `docker ps` and `docker logs` helped me become more comfortable with the terminal. This laboratory gave me more practical experience managing a cloud service from the command line.
