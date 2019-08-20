##Pull jdk11 from DockerHub
FROM openjdk:11
##Specify the work directory
WORKDIR usr/src/rabbit-mq
##Add the jar file to be executed
ADD .target/consumer-0.0.1-SNAPSHOT.jar /usr/src/consumer-0.0.1-SNAPSHOT.jar
##ENTRYPOINT allows you to configure a container that will run as an executable
ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-jar","consumer-0.0.1-SNAPSHOT.jar"]
