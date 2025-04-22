# Spring Boot Project with Maven - S04T01N01

This is a Spring Boot project built with Maven as the dependency manager.

## Requirements

* Java JDK (minimum version 11)
* Maven installed
* Postman (or a similar HTTP client) for testing the API endpoints

## How to run the application

1.  Navigate to the root directory of the project in your terminal.
2.  Run the Maven command to start the application:
    ```bash
    mvn spring-boot:run
    ```
3.  The application will be accessible at `http://localhost:9000`.

## API Endpoints

This API has been tested using Postman.

* `GET /HelloWorld`: Returns a greeting with an optional "nombre" parameter (default is "UNKNOWN").
    * **Example (Postman):** Send a GET request to `http://localhost:9000/HelloWorld` or `http://localhost:9000/HelloWorld?nombre=YourName`.
* `GET /HelloWorld2/{nombre}`: Returns a greeting with an optional "nombre" parameter in the path.
    * **Example (Postman):** Send a GET request to `http://localhost:9000/HelloWorld2` or `http://localhost:9000/HelloWorld2/YourName`.

## Maven Commands

* `mvn clean`: Cleans the project, removing the `target` directory.
* `mvn compile`: Compiles the project.
* `mvn package`: Packages the project into a JAR or WAR file in the `target` directory.
* `mvn spring-boot:run`: Runs the Spring Boot application.
