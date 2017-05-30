# Spring Boot APPUiO Example

This is a Spring Boot Example Application

## How to deploy

### Create New OpenShift Project
```
$ oc new-project example-spring-boot
```

### Docker Build on APPUiO - Create Application and expose Service
```
$ oc new-app https://github.com/agello/example-spring-boot-helloworld.git --strategy=docker --name=agello-spring-boot-ex

$ oc expose service agello-spring-boot-ex
```

### Image from DockerHub
Take the pre built image from Dockerhub

```
$ oc new-app tomcc/example-spring-boot
```


