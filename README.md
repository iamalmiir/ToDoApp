# TaskMaster

This is a simple and intuitive To Do App that allows you to create and manage tasks easily.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)

# Usage

## Requirements

- JDK 11 or higher
- Maven 3.6.3 or higher

## Installation

Sure, here are the installation instructions for your WebFlux functional To Do App:

1. Clone the repository to your local machine.
2. Make sure you have Java 11 or higher installed on your machine.
3. Make sure you have Maven installed on your machine.
4. In the terminal, navigate to the project root directory.
5. Run the command `mvn clean package` to build the project and generate a jar file.
6. Run the command `java -jar target/restful-spring-1.0-SNAPSHOT.jar` to start the server.
7. The server will be running on `http://localhost:8080/`.

Note: You might need to configure your database connection in the `application.properties` file
before running the project.

## Running the application

1. Run the application: `java -jar target/<jar-file-name>.jar`
2. The application will run on `http://localhost:8080`

## API Endpoints

- GET `/tasks`: Retrieve all tasks.
- GET `/tasks/{id}`: Retrieve a task by ID.
- POST `/tasks`: Create a new task.
- PUT `/tasks/{id}`: Update a task.
- DELETE `/tasks/{id}`: Delete a task.

### Sample Request Body (for POST and PUT requests)

```json
{
  "title": "Task title",
  "taskDescription": "Task description",
  "completed": false
}
```

### Sample Response Body (for GET, POST, and PUT requests)

```json
{
  "id": "48ad4c4b-4f8c-4ca6-b5f5-5f6c5e23806c",
  "title": "Task title",
  "taskDescription": "Task description",
  "completed": false
}
```