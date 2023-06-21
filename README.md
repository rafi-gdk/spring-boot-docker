This application provides all Customer Information

Pre Requisites : Java 19 and Gradle 7.6 and Postgres

Install Postgres:
> docker run --name postgresql -e POSTGRES_USER=postgres -e POSTGRES_PASSWORD=123456789 -p 5432:5432 -d postgres

Used topics:

1.Http all Requests

2.Form Validations

3.PathVariable Validations

4.Postgres db by setting up all required info in application.yml variables

5.Used Global Exception handler

6.docker images

------------------------------------------------------------------------------------------------------------------------------------------
Steps to Execute:
1. open powershell terminal and execute below commands

    > cd D:\MyWork\my-git-hub\spring-boot-docker
    
    > ./gradlew clean build
    
    > docker build -f ./docker-images/Dockerfile -t customer-service:latest .
    
    > docker run --name customer-service -p 1001:1001 -t customer-service:latest

------------------------------------------------------------------------------------------------------------------------------------------
some of docker commands:
> docker -–version

> docker images

> docker run [image id]

> docker ps

> docker stop [container id]

> docker kill [container id]

> docker rm [container id]

> docker login

> docker push

> docker build -f [folder path where we have docker file] -t [name for repository:tag]

------------------------------------------------------------------------------------------------------------------------------------------