# Cloud Infrastructure Components

## Introduction

Cloud infrastructure is made up of different resources that work together to provide computing services. In the KillerCoda Linux environment, we can observe resources such as compute, storage, networking, and the operating system. These resources are also important parts of a cloud computing environment.

## 1. Compute Resources

### Purpose

Compute resources provide the processing power needed to run applications, execute commands, and perform different workloads.

### Importance in Cloud Computing

Compute resources are important because applications and services need processing power to work properly. In cloud computing, virtual computing resources can also be adjusted depending on the workload or requirements of the users.

### KillerCoda Linux Environment

In the KillerCoda environment, the compute resource is provided by a virtual CPU. Based on the investigation, the server has an **Intel Xeon E312xx (Sandy Bridge, IBRS update)** processor with **1 CPU core**.

## 2. Storage Resources

### Purpose

Storage resources provide space for the operating system, applications, configuration files, and other data.

### Importance in Cloud Computing

Storage is important in cloud computing because applications and services need a place where they can save and access data. Cloud storage also allows organizations to manage their data without relying only on physical storage devices.

### KillerCoda Linux Environment

In the KillerCoda environment, the main storage resource is **`/dev/vda1`**. It has a capacity of **19 GB** and is mounted on **`/`**, which is the root directory of the Linux operating system. Other mounted file systems include **`/dev/vda16`** mounted on **`/boot`** and **`/dev/vda15`** mounted on **`/boot/efi`**.

## 3. Networking Resources

### Purpose

Networking resources allow computers, servers, applications, and users to communicate with each other.

### Importance in Cloud Computing

Networking is important in cloud computing because cloud services need network connections to communicate with users, other servers, and different cloud resources. Good network connectivity allows applications and services to exchange information properly.

### KillerCoda Linux Environment

In the KillerCoda environment, the server has the hostname **`ubuntu`** and the IP addresses **`172.30.1.2`** and **`172.17.0.1`**. These network addresses allow the Linux environment to connect and communicate within its network environment.

## 4. Operating System

### Purpose

An operating system manages the computer's hardware resources and provides an environment where applications and other software can run.

### Importance in Cloud Computing

The operating system is important in cloud computing because it manages resources such as the CPU, memory, storage, and networking. It also provides the foundation needed for applications and other workloads to operate.

### KillerCoda Linux Environment

The KillerCoda environment is running **Ubuntu 24.04.4 LTS** with the **6.8.0-136-generic** kernel. Ubuntu provides the operating environment for the virtual server and manages its available computing, storage, and networking resources.

## Conclusion

The KillerCoda Linux environment shows how different cloud infrastructure components work together. The compute resource provides processing power, storage provides space for data and system files, networking allows communication, and the operating system manages these resources. This investigation helped demonstrate how even a virtual Linux server depends on these components to provide a functional computing environment.
