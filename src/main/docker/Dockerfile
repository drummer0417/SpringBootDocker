FROM openjdk:8-jdk-alpine

VOLUME /tmp
ADD maven/spring-boot-docker-${project.version}.jar myapp.jar
RUN sh -c 'touch /myapp.jar'
ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-jar","/myapp.jar"]
