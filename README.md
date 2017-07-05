## Getting started
### Install docker, docker-machine, docker-compose

[Docker docs](https://docs.docker.com/)

## docker command

### start docker-machine

```
docker-machine start default
```

### docker setting

```
vi ~/.profile

export DOCKER_CERT_PATH=~/.docker/machine/machines/default/
export DOCKER_TLS_VERIFY="1"
export DOCKER_MACHINE_NAME="default"
export DOCKER_HOST="tcp://192.168.99.100:2376"
```

### build

```
docker-compose build
```

### up
in rubydock-localdev directory
```
docker-compose up
```

### access

```
docker-machine ip default
```

Sample: 
https://192.168.99.100

## Rails with docker

### Containers list

```
docker ps
```
Image rubydocklocaldev_rails must have. 

### Rails env

```
docker exec -it CONTAINER_ID bash
```

You can use `rails s`, `rails c` same your local. 
