# Assignment

Welcome to the assignment section for DevOps. We understand that time and resources are limited. Hence the assignments are broken into few levels. 

## Context

The sample application is a simple Spring Boot application that helps in storing the detail of the employees. It exposes REST API to CRUD on employee entity. The data is stored in an in memory database (which means that data stored in the database will not survive a server/app restart). 

### Prerequisites
1. Java 8
2. Maven 3 
3. Git Client (to check out code)
4. Postman (to invoke the API of the application)

Once checked out, use following commands to build and run the application on local machine.

```
 cd my-app
 mvn clean install
 cd target
 java -jar my-app-0.0.1-SNAPSHOT.jar
```

There is a [postman collection](DevOps-Assessment.postman_collection.json). Feel free to use and extend the same to test the API behaviour.

#### Level - 1 : Dockerize the application
1. Create a Dockerfile for the application
2. Build the image 
3. Run the image

#### Level - 2 : Build a CD pipeline
1. Create a CD pipeline in Jenkins CI server (or any other CI server of your choice)
2. As part of the pipeline, 
    1. Check out the code
    2. Build it
    3. Test using SonarQube (optional) 
    4. Test it
    5. Create Docker image of the same
    6. Push to Docker Hub
    7. Notify once the build is completed

#### Level - 3 : Provision an environment
1. Either manually or through code (like through usage of Terraform) provision the environment 

#### Level - 4 : Deploy the solution
#### Level - 5 : Monitor the solution 