# You can change this base image to anything else
# But make sure to use the correct version of Java
# Changed from adoptopenjdk/openjdk17:alpine-jre to eclipse-temurin:17-jre-alpine
# Eclipse Temurin is the new name for AdoptOpenJDK.
FROM eclipse-temurin:17-jre-alpine

# Simply the artifact path
ARG artifact=target/spring-boot-web.jar

WORKDIR /opt/app

COPY ${artifact} app.jar

# This should not be changed
ENTRYPOINT ["java","-jar","app.jar"]
