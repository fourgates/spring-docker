# Spring Docker Project 

## To Run
docker run -p 8080:8080 -t fourgates/gs-spring-boot-docker --name spring

## To Build a New Image
mvn install dockerfile:build

## To Run with Profil
docker run -e "SPRING_PROFILES_ACTIVE=prod" -p 8080:8080 -t fourgates/gs-spring-boot-docker --name spring

## To Debug
docker run -e "JAVA_OPTS=-agentlib:jdwp=transport=dt_socket,address=5005,server=y,suspend=n" -p 8080:8080 -p 5005:5005 -t springio/gs-spring-boot-docker --name spring


https://spring.io/guides/gs/spring-boot-docker/