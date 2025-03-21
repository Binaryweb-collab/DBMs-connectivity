CRUD App Backend with Express.js and MySQL

Overview

This project is a backend server for a CRUD (Create, Read, Update, Delete) application using Node.js, Express.js, and MySQL. The API is designed to manage user data and can be tested using Postman.

Prerequisites

Ensure you have the following installed:

Node.js (for backend development)

MySQL Server (for database management)

Postman (for API testing)

Git (if cloning from a repository)

Installation Steps

Clone the Repository

git clone <repository_url>
cd <repository_name>

Install Dependencies

npm init -y
npm install express cors mysql body-parser

Setup MySQL Database

Open MySQL Server and run the following SQL commands:

CREATE DATABASE crud_app;
USE crud_app;

CREATE TABLE users (
    id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(100),
    email VARCHAR(100) UNIQUE,
    password VARCHAR(255)
);

Update the server.js file with your MySQL credentials if needed.

Running the Server

Navigate to the backend folder and start the server:

cd backend1
node server.js

Running the Frontend

Open index.html in VS Code.

Click on Live Server to run the frontend.

API Endpoints

Method

Endpoint

Description

GET

/users

Fetch all users

POST

/users

Add a new user

PUT

/users/:id

Update a user

DELETE

/users/:id

Delete a user

Project Customization

In this project, you can modify the frontend, backend, and database as needed. Feel free to clone the repository and modify the code.

Next Steps

Implement authentication (JWT, bcrypt for password hashing)

Connect to a frontend (React, Vue, Angular)

Deploy the backend to a server (Heroku, AWS, etc.)

Author

Santhosh Kumar

Happy Coding! 🚀