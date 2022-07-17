# Patika-Emlakjet-Graduation


# About the project
It is a web application where users can post advert in the real estate sector. To create a registration, tokens are purchased with Email and Password.
Thanks to the Gateway, the desired CRUD operations are authorized via this token. The desired service can be accessed through the Gateway.

Within the scope of this project, 5 services have been prepared.

- Admin Service
- Banner Service
- Cloud Gateway
- Emlakjet
- Report Service

### Getting started
Make sure port 5432,5672,15672,8080,8081,8082,8083,8084 are not in use

### Installing & Running Emlakjet Microservices
    
    mvn clean install
    docker-compose up

    # try forcing a image rebuild
    docker-compose up --build --force-recreate


### To execute the API's through the gateway
    1) localhost:8080/login 
    2) localhost:8080/advert-api/** -> emlakjet
    3) localhost:8080/banner-api/** -> emlakjet-banner 
    4) localhost:8080/report-api/** -> emlakjet-report
    5) localhost:8080/admin-api/** -> emlakjet-admin
  
    
### Basic use cases
#### 1) Signup a new user 
#### 2) Login with the created user to get authentication token
#### 3) Create an address 
#### 4) Create a property 
#### 5) Create a advert 
    
 ### You can see the api documentation on the swagger page after you run all the services. Swagger will be available on;
 
  ```
  Gateway/Auth   -> http://localhost:8080/swagger-ui.html
  Emlakjet       -> http://localhost:8081/swagger-ui.html
  Banner         -> http://localhost:8082/swagger-ui.html
  Report         -> http://localhost:8083/swagger-ui.html
  Admin          -> http://localhost:8084/swagger-ui.html
  ```
  
  
  
### Arcitechture diagram

### ER diagram

### Considerations During the Writing of the Project

- It has been tried to make sure that the code is clean, understandable and easy to read.
- It has been tried to be written in accordance with the code structure. It was created taking into account the layered architecture. 
- This project has been tried to be done in accordance with the microservice architecture.
- Exception Handling have been tried to be used.
- Programming principles (SOLID etc.) were tried to be taken into account.


### Future Work

- Logging and Exception Handling can be diversified to make them more inclusive across the whole code.
- Logging operations written to a file or database.
- Instead of using a common database, each service can be connecting to its own database to be more secure.
- Design patterns can be used.
- The unit test should be developed by writing new tests for all services and all cases of these services' methods.
- A suitable frontend can be written.



