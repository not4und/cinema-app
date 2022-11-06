# cinema-app
This is a prototype of cinema web application (only backend side) for a movie theatre. We have two general roles of user: `USER(as viewer)` and `ADMIN`.
### Endpoints
#### For non-logged in
`POST` /register  
`GET` /cinema-halls  
`GET` /movies  
`GET` /movie-sessions/available  
#### USER
`POST` /orders/complete  
`PUT` /shopping-carts/movie-sessions  
`GET` /orders  
`GET` /shopping-carts/by-user  
#### ADMIN
`POST` /cinema-halls  
`POST` /movies  
`POST` /movie-sessions  
`PUT` /movie-sessions/{id}  
`DELETE` /movie-sessions/{id}  
`GET` /users/by-email  
## Project structure
#### Levels
`DAO` Data access layer - access to the database (Hibernate API)  
`Service` Application layer - main logic of the application  
`Controller` Presentation layer - communication with a user (Spring API)  
#### Technologies
`Java` jdk-11  
`Maven`  
`Hibernate` 5.4.27.Final  
`Spring` (Core, MVC, Security) 5.2.2.RELEASE   
`MySQL` 8.0 (recommend to use)  
`Apache Tomcat` 9.0.65  
`Postman` for testing
## How to start the application
1. Install and configure Apache Tomcat(v9.0.65)
2. Install MySQL 8.0 with MySQL Workbench
3. Fill some fields in the /resources/db.properties
4. Run the application
