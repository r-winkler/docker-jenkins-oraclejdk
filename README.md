# Jenkins 

This is a docker Jenkins container based on my ubuntu-oraclejdk image.

<img src="http://jenkins-ci.org/sites/default/files/jenkins_logo.png"/>

The following additional software is installed:

* Maven
* Git
* Nano
* npm
* Jenkins Plugins
	* greenballs


## Installation

```
docker pull renewinkler/jenkins-oraclejdk
```

## Build

```
docker build . -t jenkins-oraclejdk
```


## Launch

```
docker run -itd -p 8080:8080 --name jenkins renewinkler/jenkins-oraclejdk
```


## Usage

```
http://192.168.99.100:8080
```


## Connect to Server

```
docker exec -it jenkins /bin/bash
```
