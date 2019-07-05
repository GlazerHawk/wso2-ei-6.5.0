# Project Title
Docker project wso2 Enterprise Integrator 6.5.0

## Description
This project is an isolated part of a bigger project to learn Wso2 EI 6.5.0.
In folder dockerfiles there is an Dockerfile that generates an docker image that has an Wso2 EI environment inside it.

## Getting Started
You can clone this repository to your local and docker run WSO2-EI-Dockerfile to generate a docker image
or you can pull it directly from dockerhub [docker push glazerhawk/wso2-ei-6.5.0:tagname](https://cloud.docker.com/u/glazerhawk/repository/docker/glazerhawk/wso2-ei-6.5.0).

### Dependencieso
To run a dockerfile you only need Docker so:
* Docker

### Installing
Install docker on ubuntu:18.04
* Update you ubuntu
```
sudo apt-get update
```
* Uninstall old version of docker
```
sudo apt-get remove docker docker-engine docker.io
```
* Install docker
```
sudo apt install docker.io
```
* Start docker
```
sudo systemctl start docker
sudo systemctl enable docker
```
* Give docker sudo permission to execute docker without sudo
```
sudo gpasswd -a $USER docker
```
### Executing program
* Building and running a docker image
```
docker build -f WSO2-EI-Dockerfile -t selflearning/wso2-ei-6.5.0:v1 .
docker run -it  selflearning/wso2-ei-6.5.0:v1 /bin/bash 
```
* running the containter with a volume
```
docker run -v ~/folderVolumeLocal:/nameFolderInsideContainer -it selflearning/wso2-ei-6.5.0:v1 /bin/bash

```

## Authors
* GlazerHawk
* MaykMoreira

## Version History

* 0.1
    * Initial release
