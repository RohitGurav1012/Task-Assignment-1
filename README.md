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


SQL :
create database userdb

use userdb

CREATE TABLE users (
    id INT AUTO_INCREMENT PRIMARY KEY,
    username VARCHAR(255) NOT NULL,
    contact_number VARCHAR(15) NOT NULL,
    city VARCHAR(255) NOT NULL
);

INSERT INTO users (username, contact_number, city) VALUES
('Munni', '8390251012', 'Mumbai'),
('Chuhi', '7045635498', 'Mumbai'),
('Jui', '9874563211', 'Mumbai'),
('Jasmin', '1234567891', 'Kolhapur'),
('Rashmika', '5432109876', 'Kokan'),
('Kavya', '4321098765', 'Malvan'),
('Vaishnavi', '3210987654', 'Uttar Pradesh'),
('Apeksha', '2109876543', 'Mumbai'),
('Srushti', '1098765432', 'Guwhati'),
('Rukmini', '1987654321', 'Kolhapur'),
('Komal', '8390251012', 'Mumbai'),
('Radha', '7045635498', 'Mumbai'),
('Poonam', '9874563211', 'Mumbai'),
('Prerna', '1234567891', 'Kolhapur'),
('Priyanka', '5432109876', 'Kokan'),
('Roshni', '4321098765', 'Malvan'),
('Kajal', '3210987654', 'Uttar Pradesh'),
('Sakshi', '2109876543', 'Mumbai'),
('Arya', '1098765432', 'Guwhati'),
('Pooja', '1987654321', 'Kolhapur');


