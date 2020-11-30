
># DevOps with Docker and Kubernetes 
>### IT CS3530 UNIX Operating Systems
>### Simon Welge, SAWGZQ
## Topic: DevOps With Docker and Kubernetes
I chose Docker and Kubernetes because I think containerization is a really interesting technology that will only be used more and more frequently in the future. I also do lots of webdev stuff, so being able to build a container and then spin up an aws instance with almost no configuration is really appealing. For my final project, I would like to get multiple different containers running docker and use kubernetes to host and manage them. But first, I must research what Docker/Kubernetes are.
## Research: Docker

### What is Docker?
Docker is a set of platform-as-service products that use operating system level virtualization to deliver software in packages called containers. These containers run on the Docker engine, which runs on the operating system.
### History of Docker
Docker was founded in a 2010 Startup incubator group and launched in 2011. It then was later released to the public at PyCon in 2013
### What is a container?
We have already established that Docker is a way to virtualize operating systems but we haven't touched on containers fully. Docker's definition of a container is as such:
>A container is a standard unit of software that packages up code and all its dependencies so the application runs quickly and reliably from one computing environment to another. A Docker container image is a lightweight, standalone, executable package of software that includes everything needed to run an application: code, runtime, system tools, system libraries and settings.  

The idea is that instead of using an entire virtual machine for your application or webserver, you can containerize it; and thus, save on resources to run more applications.  
Below are visualizations of how containerization is different than using virtual machines.

![enter image description here](https://zdnet2.cbsistatic.com/hub/i/r/2017/05/08/af178c5a-64dd-4900-8447-3abd739757e3/resize/770xauto/78abd09a8d41c182a28118ac0465c914/docker-vm-container.png)
##### Containerized applications take up less space, and don't require a guest operating system for each.
## Research: Kubernetes
### What is Kubernetes? 
Kubernetes, also known as k8, is an open source system for automatically deploying, scaling and managing containerized applications. Where docker was a much lower-level development tool, Kubernetes is a deployment tool that can manage all of your containers. 
![enter image description here](https://m-square.com.au/wp-content/uploads/2019/10/Docker-Kubernetes-together-4-1030x580.png)
## Application: Build, Deploy, Manage Docker Webserver with Kubernetes
### Summary
In this section, I will attempt to build some sort of webserver that I can run inside a docker container and manage with Kubernetes. To do this, I will need to:
 1. Create a docker container

