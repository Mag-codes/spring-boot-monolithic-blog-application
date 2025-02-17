# Spring Boot Blog Application

This is a complete application built with Java Spring Boot, designed to demonstrate the capabilities of Spring Data JPA, Thymeleaf, and Spring Security. The application follows the Model-View-Controller (MVC) architecture and provides a platform for users to create, read, update, and delete blog posts.

## Features

- User authentication and authorization
- Role-based access control (User and Admin roles)
- CRUD operations for blog posts
- H2 database for development and PostgreSQL for production
- Responsive web interface using Thymeleaf
- RESTful API for image handling

## Technologies Used

- Java 21
- Spring Boot 3.1.5
- Spring Data JPA
- Thymeleaf
- Spring Security
- PostgreSQL
- Maven

## Development Instructions

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/yourusername/spring-boot-blog-application.git
   cd spring-boot-blog-application
   ```

2. **Build the Application**:
   You can build the application using Maven. Make sure you have Maven installed on your machine.
   ```bash
   mvn clean package
   ```

3. **Run the Application**:
   You can run the application using the following command:
   ```bash
   mvn spring-boot:run
   ```

4. **Access the Application**:
   Open your web browser and navigate to `http://localhost:8080` to access the application.

## Built-in Accounts and Constraints

- **User Account**:
  - Email: `user.user@domain.com`
  - Password: `password`
  - Permissions: Can create, read, and update posts.

- **Admin Account**:
  - Email: `admin.admin@domain.com`
  - Password: `password`
  - Permissions: Can create, read, update, and delete posts.

- **Anonymous Account**:
  - Permissions: Can only read posts.

## Database Configuration

The application uses PostgreSQL for production. You can configure the database connection in the `src/main/resources/application.properties` file. For development, the H2 database is enabled.

### Example PostgreSQL Configuration:
