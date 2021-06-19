# Django REST Framework & Docker
## Docker
###  Docker is a way to isolate and run entire applications. In Docker the entire development environment is isolated: programming language, software packages, databases so  it doesn’t matter if you are using a Mac, Windows, or Linux computer anymore.
### Docker is a Linux containers which are a type of virtualization specifically virtual machines. virtual machines are complete copies of a computer system from the operating system on up. Virtual environments are used to isolate Python software packages locally.
## Install Docker
### To install Docker we need to download the desktop app on our computer and create a free account. Once Docker is done installing we can confirm the correct version is running. It should be at least version 19.
```
$ docker --version
Docker version 19.03.5, build 633a0ea
```
### Docker Compose is an additional tool that is automatically included with Mac and Windows downloads of Docker. However if you are on Linux, you will need to add it manually using `sudo pip install docker-compose` command after your Docker installation is complete.
## Images and Containers
### Images and containers are the two fundamental concepts to grasp when you start with Docker. An image is a snapshot in time of what a project contains. A container is a running instance of the image.
## Library Website and API