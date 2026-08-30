# Cloud Infrastructure Components

Cloud infrastructure consists of different resources that work together to support applications, services, and data in a cloud environment. During the investigation of the KillerCoda Linux environment, I observed examples of compute, storage, networking, and operating system resources.

## Compute Resources

**Purpose:**  
Compute resources provide the processing power required by a computer or server to execute commands, run applications, and process different workloads. These resources mainly include the processor or CPU and its available cores.

**Importance in Cloud Computing:**  
Compute resources are important in cloud computing because every application and service needs processing power to operate. The amount of available compute resources can affect how efficiently a cloud server performs its tasks. Cloud environments can also provide additional computing resources when workloads increase.

**KillerCoda Linux Environment:**  
In my KillerCoda environment, the compute resource is represented by an Intel Xeon E312xx (Sandy Bridge, IBRS update) processor. Using the `lscpu` command, I identified that the environment has one CPU and one CPU core. This processor is responsible for executing the Linux commands and other tasks performed inside the cloud server.

## Storage Resources

**Purpose:**  
Storage resources provide space where the operating system, applications, files, and other data can be stored. They allow information to remain organized and accessible to the system when it is needed.

**Importance in Cloud Computing:**  
Storage is an essential part of cloud infrastructure because applications and services need a location where their data can be kept. Cloud servers also require storage for system files, application files, logs, and other information. Proper storage management helps ensure that sufficient space is available for different workloads.

**KillerCoda Linux Environment:**  
I investigated the storage resources of the KillerCoda environment using the `df -h` command. The main `/dev/vda1` file system has a total capacity of 19 GB, with 13 GB available during my investigation. The command also displayed several mounted file systems, including `/`, `/boot`, `/boot/efi`, `/run`, `/dev/shm`, and `/run/lock`. These show how storage is organized and made accessible within the Linux environment.

## Networking Resources

**Purpose:**  
Networking resources provide communication and connectivity between computers, servers, users, applications, and other resources. They allow data to travel between connected systems through a network.

**Importance in Cloud Computing:**  
Networking is important because cloud resources must communicate with users and other systems. Without network connectivity, users would not be able to access cloud-hosted services, and different cloud resources would not be able to exchange information with one another.

**KillerCoda Linux Environment:**  
I investigated the networking information of the KillerCoda server using the `hostname` and `hostname -I` commands. The hostname of my server is `ubuntu`, while the IP addresses displayed were `172.30.1.2` and `172.17.0.1`. The hostname identifies the server by name, while the IP addresses are used to identify it within its network environment.

## Operating System

**Purpose:**  
The operating system manages the hardware and software resources of a computer. It provides the environment where users can execute commands, manage files, run applications, and interact with system resources.

**Importance in Cloud Computing:**  
An operating system is important in cloud computing because cloud servers need a platform that can manage compute, memory, storage, networking, and software processes. It also provides the tools and services needed to operate and administer a cloud server.

**KillerCoda Linux Environment:**  
My KillerCoda cloud server runs Ubuntu 24.04.4 LTS (Noble Numbat) with Linux kernel version 6.8.0-138-generic. I identified the operating system using the `cat /etc/os-release` command and checked the kernel version using `uname -r`. This Linux environment allowed me to use terminal commands to investigate and manage the available cloud infrastructure resources.
