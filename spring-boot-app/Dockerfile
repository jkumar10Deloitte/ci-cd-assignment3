#base image
FROM adoptopenjdk/openjdk11:alpine-jre

ARG artifact=target/spring-boot-web.jar

#workdirectory 
WORKDIR /opt/app

COPY ${artifact} app.jar

# Final step || entry point
ENTRYPOINT ["java","-jar","app.jar"]
