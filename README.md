# Jenkins with Docker

## Prerequirement

```sh
docker-compose >= 1.10.0
```
Install docker-compose (linux):
```sh
curl -L https://github.com/docker/compose/releases/download/1.21.2/docker-compose-$(uname -s)-$(uname -m) -o /usr/local/bin/docker-compose
```

## Installation

just run
```sh
docker-compose up -d
```

or create own image for useing docker in jenkins

```sh
docker-compose -f docker-compose.build.yml up -d --build
```


After all, run this:
```sh
docker exec -it jenkins cat /var/jenkins_home/secrets/initialAdminPassword
```
