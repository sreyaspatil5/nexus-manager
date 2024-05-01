# Nexus Manager

Nexus Manager is a Spring Boot application designed to manage admins and users in a system. It provides RESTful APIs for performing CRUD (Create, Read, Update, Delete) operations on admins and users.

## Features

- **Admin Management**: APIs to handle CRUD operations for admin entities.
- **User Management**: APIs to handle CRUD operations for user entities.
- **Association**: Ability to associate users with admins.

## Technologies Used

- **Spring Boot**: Framework for building Spring-based applications.
- **Spring Data JPA**: Simplifies data access through the JPA abstraction.
- **MySQL Database**: Used for persistent storage of admin and user data.
- **Hibernate Validator**: Provides flexible and powerful object validation capabilities.
- **Maven**: Dependency management and project build tool.
- **JUnit**: Framework for unit testing.

## API Endpoints

### Admins

- `GET /api/admins`: Retrieve all admins.
- `GET /api/admins/{id}`: Retrieve admin by ID.
- `POST /api/admins`: Create a new admin.
- `PUT /api/admins/{id}`: Update an existing admin.
- `DELETE /api/admins/{id}`: Delete an admin by ID.

### Users

- `GET /api/users`: Retrieve all users.
- `GET /api/users/{id}`: Retrieve user by ID.
- `POST /api/users`: Create a new user.
- `PUT /api/users/{id}`: Update an existing user.
- `DELETE /api/users/{id}`: Delete a user by ID.
- `POST /api/users/admin/{adminId}`: Create a new user associated with the specified admin.

## Setup Instructions

1. **Clone the Repository**: `git clone <repository-url>`
2. **Database Configuration**:
   - Configure MySQL database settings in `application.properties`.
3. **Build and Run**:
   - Navigate to the project directory and run `mvn spring-boot:run`.
4. **Access APIs**:
   - Access the APIs using a REST client such as Postman or cURL.

## Contributing

Contributions are welcome! If you'd like to contribute to this project, please fork the repository and submit a pull request.
