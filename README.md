# mydocreaderDocker
Docker Compose to start or stop Service Registry, Gateway Service, File Service

## How to install Docker on Amazon Linux 2

### Install docker, run:

``` bash
$ sudo yum install docker
```

### Add group membership for the default ec2-user so you can run all docker commands without using the sudo command:

``` bash
$ sudo usermod -a -G docker ec2-user
$ id ec2-user
```

### Reload a Linux user's group assignments to docker w/o logout

``` bash
$ newgrp docker
```

### Need docker-compose too? Try any one of the following command:

### 1. Get pip3 

``` bash
$ sudo yum install python3-pip
```

### 2. Then run any one of the following

``` bash
$ sudo pip3 install docker-compose # with root access
```

### OR #

``` bash
$ pip3 install --user docker-compose # without root access for security reasons
```

### Enable docker service at AMI boot time:

``` bash
sudo systemctl enable docker.service
```

### Start the Docker service:

``` bash
sudo systemctl start docker.service
```

## Get started

1. Go to the directory of the file docker-compose.yml
2. Place all of the jar files based on the volumes mentioned at docker-compose.yml

### Start services docker-compose.yml

``` bash
$ docker-compose up -d
```

### Stop services inside docker-compose.yml

``` bash
$ docker-compose down
```
