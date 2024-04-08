# SpringBoot Blog APP

## Product Description: 

        Users can use the app to post the blogs and than other uses can comment on the existing posts. 
        Users can also browse the posts by category. The app is only open for registered users

## App Structure:

        The app developed by three layer structure: *Controller layer, Service layer, DAO layer*. 
        
The REST APIs are created at the controller class to hold the http requests and return the code response; The service layer operates the business logic of the app;The DAO(repository) layer is responsible to communicate with database.

The app also uses postman to test the API and utilize DTOs to transmit data between client and server.JSON works as a message exchange format between the client and server. Besides, I decouple the class by setting the service class as interface and using serviceImpl class to implement the interface.<br>

## Technology Stack for the App:

        Java Platform: Java 17+ 
        Java Frameworks: Spring Framework and it's portfolio projects like SpringBoot, Spring Security, Spring Data JPA 
        Token based Authentication: JWT(JSON Web Token) 
        Build Tool: Maven 
        IDE: IntelliJ IDEA 
        Server: Tomcat embeded server 
        Database: MySQL database 
        REST Client: Postman 
        REST API Decumentation: SpringDoc OpenAPI 
        Cloud for Deployment: AWS Cloud 

## High Level Requirements for Blog App:

### 1.Posts Management
    Create, Read, Update and Delete Posts. Provide Pagination, Sorting and Filter support

### 2.Comments Management for Post (one to many mapping)
    Create, Read, Update and Delete Comments for Blog Posts

### 3.Category Management (one to many mapping)
    Create, Read, Update and Delete Category

### 4.Authentication and Authorization
    Register, Login and Security
- 4.1 Secure REST APIs using Database Authentication
- 4.2 Build Login Rest API and SignUp REST API
- 4.3 Use JWT token based Authentication to Secure the REST API
- 4.4 Implement Role-based security - ADMIN and User Roles

### 5.Exceptions Handling and REST API Validations
- I customize a ResourceNotFoundException and a BlogAPIException to describe specific errors, also build GlobalExceptionHandler to handle specific exceptions and return proper error response the client
- I also add a REST API validation component which is to validate the REST API request and send the validation error response to the client. For example, when the user signs up the app, the username must not be null and the email address must be in a right email format, etc

### 6.Versioning REST API and Deploying on AWS Beanstalk
- Versioning REST API by Swagger
- Deploy Blog app on AWS Cloud


