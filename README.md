User Management System
This project is a user management system implemented using Spring Boot. It provides a REST API to manage user data, including the ability to add, retrieve, update, and delete users.

Prerequisites
Before you begin, make sure that you have the following software installed on your machine:

Java 19
Maven
A database management system (such as MySQL)
Getting Started
These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.



Clone the repository:

bash
Copy code
git clone https://github.com/[your-username]/user-management-system.git
Navigate to the project directory:

sql
Copy code
cd user-management-system
Configure the database connection in the application.properties or application.yml file. By default, the project uses an in-memory database for testing purposes, but you can change it to your own database by modifying the following properties:

less
Copy code
spring.datasource.url=jdbc:mysql://localhost:3306/[database-name]
spring.datasource.username=[database-username]
spring.datasource.password=[database-password]
Build and run the project using the following Maven command:

Copy code
mvn spring-boot:run
The API will be available at http://localhost:8080. You can use a tool such as Postman to make API requests.

API Endpoints
The following API endpoints are provided:

POST /addUser: Adds a new user to the database.
GET /getUser/{userId}: Retrieves the user data for the specified userId.
GET /getAllUser: Retrieves all users from the database.
PUT /updateUserInfo: Updates the user information for the specified userId.
DELETE /deleteUser/{userId}: Deletes the user with the specified userId from the database.
Built With
Spring Boot - The framework used for building the API
Maven - Dependency management
JPA - Used for database interaction
Contributing
If you would like to contribute to this project, please create a fork and submit a pull request.

License
This project is licensed under the MIT License - see the LICENSE file for details.