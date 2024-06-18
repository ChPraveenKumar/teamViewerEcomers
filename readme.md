
# E-Commerce Platform Spring Boot Application

Welcome to the E-Commerce Platform Spring Boot Application! This project is a simple e-commerce platform built using Spring Boot and integrated with a PostgreSQL database. It provides a REST API for managing orders and order items, following OpenAPI standards.

## Table of Contents

- [Prerequisites](#prerequisites)
- [Getting Started](#getting-started)
- [API Documentation](#api-documentation)
- [Running with Docker](#running-with-docker)
- [Running Tests](#running-tests)
- [Error Handling](#error-handling)

## Prerequisites

Before you begin, ensure you have the following installed:

- Java 11 or higher
- PostgreSQL database server
- Docker (for containerization)

## Getting Started


1. Configure the database connection in `src/main/resources/application.properties`. Replace placeholders with your database credentials.

```properties
spring.datasource.url=jdbc:postgresql://localhost:5432/frontlineDB
spring.datasource.username=your-username
spring.datasource.password=your-password
```

2. Build and run the application using Gradle or Maven:

```bash

# Using Maven
./mvnw spring-boot:run
```

The application will start at http://localhost:8080.

## API Documentation

You can access the API documentation using Swagger UI:

- Swagger UI: [http://localhost:8080/swagger-ui.html](http://localhost:8080/swagger-ui.html)

The documentation provides details about available endpoints, request/response formats, and allows you to interact with the API directly.

## Running with Docker

To run the application in a Docker container, follow these steps:

1. Build the Docker image:

```bash
docker build -t e-commerce-app .
```

2. Run the Docker container:

```bash
docker-compose up -d
```

The application will be accessible at http://localhost:8080.

## Running Tests

Run automated tests using the following commands:

```bash

# Using Maven
./mvnw test
```

## Error Handling

The application handles errors gracefully and returns appropriate HTTP status codes for different scenarios.
