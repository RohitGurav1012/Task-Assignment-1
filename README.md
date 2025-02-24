# User Details Web Application

## Description
A web application to display user details with filtering, pagination, and sorting functionality.

## Technologies Used
- **Frontend**: HTML, Thymeleaf
- **Backend**: Java (Spring Boot)
- **Database**: MySQL

## Features Implemented
- Display user details from the database.
- Filtering by username, contact number, and city.
- Pagination (5 records per page) with Next/Previous buttons.
- Sorting functionality.

## Database Schema
```sql
CREATE TABLE users (
    id INT AUTO_INCREMENT PRIMARY KEY,
    username VARCHAR(255) NOT NULL,
    contact_number VARCHAR(15) NOT NULL,
    city VARCHAR(255) NOT NULL
);


Running the Application
Start MySQL and create the database.
Update application.properties with your database credentials.
Run the Spring Boot application.
Access the UI at: http://localhost:8080/users?username=&contactNumber=&cities=malvan
The username & Contact Number must be entered manually in the url.
