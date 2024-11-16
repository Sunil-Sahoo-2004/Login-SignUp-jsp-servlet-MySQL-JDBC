# Login-SignUp Web Application

This project is a basic web application that allows users to sign up and log in using JSP, Servlets, MySQL, and JDBC. It provides basic authentication and user management functionality.

## Features

- User Registration (Sign Up)
- User Login
- Password Hashing for Security
- Session Management
- Input Validation

## Technologies Used

- **Frontend:** JSP (JavaServer Pages), HTML, CSS
- **Backend:** Java Servlets
- **Database:** MySQL
- **JDBC:** Java Database Connectivity for MySQL communication
- **Server:** Apache Tomcat

## Project Structure

├── src │ ├── com.example.dao │ │ └── UserDAO.java │ ├── com.example.model │ │ └── User.java │ ├── com.example.controller │ │ └── LoginServlet.java │ │ └── SignupServlet.java │ └── web.xml ├── web │ ├── index.jsp │ ├── login.jsp │ ├── signup.jsp │ ├── dashboard.jsp └── README.md


## Setup Instructions

### Prerequisites

- Apache Tomcat Server
- MySQL Database
- JDK 8 or above
- IDE (e.g., Eclipse or IntelliJ)

### Database Setup

1. Install MySQL and create a database:

```sql
CREATE DATABASE user_db;
USE user_db;

CREATE TABLE users (
    id INT PRIMARY KEY AUTO_INCREMENT,
    username VARCHAR(100) NOT NULL,
    password VARCHAR(100) NOT NULL
);

2. Insert sample data:
INSERT INTO users (username, password) VALUES ('admin', 'password');

```
# Configuration
Configure MySQL credentials in UserDAO.java:

private String jdbcURL = "jdbc:mysql://localhost:3306/user_db";
private String jdbcUsername = "root";
private String jdbcPassword = "your_password";


## Add your database driver to the WEB-INF/lib folder (e.g., mysql-connector-java.jar).
### Running the Project
- Clone or download the project.
- Import it into your IDE.
- Build and run on an Apache Tomcat server.
- Access the web app at http://localhost:8080/your-app-name/.
- 
### Application Endpoints
- Sign Up: /signup.jsp
- Login: /login.jsp
- Dashboard (protected): /dashboard.jsp

## License
This project is open source and available under the MIT License.
- Feel free to customize this template based on your project details and add any additional instructions or dependencies as needed.

## Contact

For any inquiries or questions, please contact:

- **Name:** Sunil Sahoo
- **Email:** sunilsahoo1525@gmail.com
- **Phone:** 7029003624

