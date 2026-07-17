# Support Ticket Management System

## Overview

Support Ticket Management System is a Spring Boot application developed to manage support tickets efficiently. The system provides REST APIs for creating, updating, retrieving, and deleting support tickets.

The project demonstrates the use of:

- Spring Boot
- Spring Data JPA
- Hibernate
- MySQL
- Spring Security
- Thymeleaf
- Swagger OpenAPI
- Validation
- Exception Handling
- Dependency Injection

---

## Technologies Used

- Java 26
- Spring Boot 4.1.0
- Spring Data JPA
- Hibernate
- MySQL
- Spring Security
- Thymeleaf
- Swagger OpenAPI
- Maven

---

## Features

### Ticket Management

- Create Support Ticket
- View All Tickets
- View Ticket By ID
- View Tickets By Category
- Update Ticket
- Partially Update Ticket
- Delete Ticket

### Validation

- Required title validation
- Estimated hours validation
- Ticket code format validation

### Security

- Authentication using Spring Security
- Protected REST APIs

### Exception Handling

- Custom Exception
- Global Exception Handler
- 404 Not Found Response

### Documentation

- Swagger UI Integration

---

## Project Structure

```
src/main/java

├── controller
│   ├── SupportTicketController
│   ├── SystemController
│   └── ViewController
│
├── service
│   ├── SupportTicketService
│   ├── NotificationService
│   ├── EmailNotificationService
│   └── SmsNotificationService
│
├── repository
│   └── SupportTicketRepository
│
├── entity
│   └── SupportTicket
│
├── exception
│   ├── TicketNotFoundException
│   └── GlobalExceptionHandler
│
└── config
    └── AppConfig
```

---

## Database Configuration

Database:

```sql
support_ticket_db
```

application.properties:

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/support_ticket_db
spring.datasource.username=springstudent
spring.datasource.password=springstudent
```

---

## REST APIs

### Get All Tickets

```http
GET /api/tickets
```

### Get Ticket By ID

```http
GET /api/tickets/{id}
```

### Get Tickets By Category

```http
GET /api/tickets/category/{category}
```

### Create Ticket

```http
POST /api/tickets
```

### Update Ticket

```http
PUT /api/tickets/{id}
```

### Partial Update Ticket

```http
PATCH /api/tickets/{id}
```

### Delete Ticket

```http
DELETE /api/tickets/{id}
```

---

## Swagger

Swagger UI:

```text
http://localhost:8081/swagger-ui.html
```

or

```text
http://localhost:8081/swagger-ui/index.html
```

---

## Thymeleaf Pages

Tickets Page:

```text
http://localhost:8081/tickets-page
```

Ticket Form:

```text
http://localhost:8081/ticket-form
```

---

## Custom Property

```properties
training.system.name=COOP Training System
```

Endpoint:

```text
http://localhost:8081/system-name
```

---

## Author

Mohammed AlMalki

Support Ticket Management System Project
Ejada Systems Internship Program
