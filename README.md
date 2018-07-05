# Jenkins with Docker

just run
```sh
docker-compose up -d
```

or create own image for useing docker in jenkins

```sh
docker-compose up -d --build
```


After all, run this:
```sh
docker exec -it jenkins cat /var/jenkins_home/secrets/initialAdminPassword
```
