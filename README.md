# ServiceDiscovery

## Overview
ServiceDiscovery is a Spring Boot application that serves as a Eureka server for service discovery. It allows microservices to register themselves and discover other registered services.

## Prerequisites
- Java 17
- Maven

## Getting Started

### Clone the Repository
```sh
git clone <repository-url>
cd ServiceDiscovery
```

### Build the Project
```sh
mvn clean install
```

### Run the Application
```sh
mvn spring-boot:run
```

The application will start on port 8761 by default.

## Configuration
The application can be configured using the `src/main/resources/application.properties` file. Below are the default configurations:

```ini
spring.application.name=ServiceDiscovery
server.port=8761
eureka.client.registerWithEureka=false
eureka.client.fetchRegistry=false
```

## Dependencies
The project uses the following dependencies:
- Spring Boot Starter Web
- Spring Cloud Starter Netflix Eureka Server
- Spring Boot DevTools
- Spring Boot Configuration Processor
- Lombok
- Spring Boot Starter Test

## Maven Configuration
The `pom.xml` file includes the necessary configurations and dependencies for the project. It inherits from the `spring-boot-starter-parent` and includes overrides to prevent unwanted inheritance of `<license>` and `<developers>` elements.

## License
This project is licensed under the terms specified in the `pom.xml` file.

## Developers
For information about the developers, refer to the `pom.xml` file.

## Additional Information
For more details, refer to the `HELP.md` file.