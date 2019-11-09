# Benefits of using Docker

## Speed and size

## Reproducible and portable builds

## Immutable and agile infrastructure

## Docker Engine and Docker Engine client

Docker is a client-server application. It consists of the daemon that does the important job: builds and downloads images, starts and stops containers and so on. It exposes a REST API that specifies interfaces for interacting with the daemon and is being used for remote management. Docker Engine accepts Docker commands from the command line, such as docker to run the image, docker ps to list running containers, docker images to list images, and so on.

The Docker client is a command-line program that is used to manage Docker hosts running Linux containers. It communicates with the Docker server using the REST API wrapper. You will interact with Docker by using the client to send commands to the server.

Docker Engine works only on Linux. If you want run Docker on Windows or Mac OS, or want to provision multiple Docker hosts on a network or in the cloud, you will need **Docker Machine**.

## Docker Machine

It's a quick way to get a new virtual machine provisioned and ready to run Docker containers. Docker Machine not only creates a new VM with the Docker Engine installed in it, but sets up the certificate files for authentication and then configures the Docker client to talk to it. In fact, when you install Docker for Windows or Mac OS, the default VirtualBox driver will be used. The following command will be executed behind the scenes:

```bash
docker-machine create --driver=virtualbox default
```
Another available driver is amazonec2 for Amazon Web Services. It can be used to install Docker on the Amazon's cloud

The list contains the following drivers at the moment:

Amazon Web Services
Microsoft Azure
Digital Ocean
Exoscale
Google Compute Engine
Generic
Microsoft Hyper-V
OpenStack
Rackspace
IBM Softlayer
Oracle VirtualBox
VMware vCloud Air
VMware Fusion
VMware vSphere

 If you want to deal with the cloud providers or just want to have common runtime environment portable between Mac OS, Windows, and Linux, you can install Docker Machine for Linux as well. 

 # Chapter 3. Understanding Images and Containers

 
