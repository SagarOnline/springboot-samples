# Read Me First
 Simple Spring Boot application 

# Getting Started

### Running Application Locally
Open a command prompt and go to directory 'springboot-samples/hello-world'. Follow below steps to run application locally,

#### Build maven application

* run command ``` mvn package ``` . This will create a runnable hello-world.jar file in target directory.

* If you want to test this application before running inside the docker then, run command 
	``` java -jar ./target/hello-world.jar```
  This will start application on port 8080. Open url 
  ``` http://localhost:8080/ ``` to test the application.

* Press Ctrl+c to close the application

#### Build Docker Image of the  application

* run command ``` docker build -t hello-world:latest  . ``` . This will create a build the docker image of the application with image name:tag  'hello-world:latest'.

* To view the docker image just created , run command ``` docker images```

#### Run application in Docker Container

* Run command to run appliation in docker container
``` docker run  --rm -it --name hello-world -p 8080:8080 hello-world:latest ``` 
This will start application on port 8080. Open url 
  ``` http://localhost:8080/ ``` to test the application.
 
* Press Ctrl+c to close the application
