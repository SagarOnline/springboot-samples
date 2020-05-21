FROM openjdk:8-jre-alpine
COPY target/hello-world.jar app.jar
ENTRYPOINT ["java","-jar","/app.jar"]
EXPOSE 8080