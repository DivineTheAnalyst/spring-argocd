FROM openjdk:21-jdk-slim

RUN apt-get update && apt-get install -y curl && rm -rf /var/lib/apt/lists/*

VOLUME /tmp

EXPOSE 8080

ADD target/spring-app.jar app.jar

ENTRYPOINT ["java","-jar","/app.jar"]