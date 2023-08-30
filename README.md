# StudentApiMongoDB
## live preview guid  https://studentapi.jamirhossain.repl.co/
#### Welcome to the StudentAPIMongoDB application! This application provides a RESTful API to manage student information using a MongoDB database. It allows you to perform basic CRUD (Create, Read, Update, Delete) operations on student records.
This code is an example of how to create a RESTful API with Express.js and MongoDB. It creates an Express.js app that listens on port 3000 and defines a route for the /students endpoint. The timeAccessMiddleware is applied to restrict access to the /students route. The middleware checks if the current time is between 9 AM and 5 PM before allowing access to the route. If the time is outside this range, the middleware returns a 403 Forbidden error.

The code also uses the cors module to enable cross-origin requests and the express.json() middleware to parse JSON in requests.

To use this code, you’ll need to install the required dependencies (express, cors, mongodb) using npm. You’ll also need to set up a MongoDB database and configure the db.js file with your database connection details.

I hope this helps you get started with creating your own RESTful API!



## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Technologies Used](#Technologies-Used)
- [Getting Started](#getting-started)
- [API Endpoints](#api-endpoints)
- [User Guide](#user-guide)
- [Contributing](#contributing)
- [License](#license)

## Introduction

The StudentAPI project aims to simplify the management of student data. It offers a RESTful API that allows you to interact with student records using HTTP requests.

## Features
- Add new student records with details such as name, age, grade, etc.
- Retrieve information about existing students.
- Update student details.
- Delete student records.
## Technologies Used

- Node.js: Backend runtime environment.
- Express: Web application framework for Node.js.
- MySQL: Relational database management system.
- HTML/CSS: For the web interface.
- JavaScript: Programming language for both backend and frontend logic.
  
## Getting Started

To start using the StudentAPI, follow these steps:

1. Clone the repository:
   ```sh
   # git clone https://github.com/your-username/your-repo.git
  ## Navigate to the project directory:
<pre>
  cd your-repo
</pre>
 ## Install dependencies:
<pre>
  npm install
</pre>
## api server start 
<pre>
  npm start
</pre>
# The API will be accessible at http://localhost:3000.
## API Endpoints
### The following API endpoints are available:
- GET /students: Retrieve a list of all students.
- GET /students/:id: Retrieve details of a specific student.
- POST /students: Add a new student record.
- PUT /students/:id: Update details of a student.
- DELETE /students/:id: Delete a student record.
# User Guide
## Retrieving Students
### To retrieve a list of all students, make a GET request to /students:
<pre>
  GET http://localhost:3000/students
</pre>

 ##  To retrieve details of a specific student, replace :id with the student's ID and make a GET request to /students/:id:
<pre>
  GET http://localhost:3000/students/1
</pre>

# Adding Students
### To add a new student record, make a POST request to /students with JSON data containing student details:
<pre>
   
  curl -X POST http://localhost:3000/students -H "Content-Type: application/json" -d '{"name": "John Doe", "age": 18, "grade": "A"}'
   
</pre>
# Updating Students
### To update a student's details, replace :id with the student's ID and make a PUT request to /students/:id with JSON data containing the updated details:
<pre>

 curl -X PUT http://localhost:3000/students/1 -H "Content-Type: application/json" -d '{"age": 19}'
   
</pre>
## Deleting Students
### To delete a student record, replace :id with the student's ID and make a DELETE request to /students/:id:
<pre>
 curl -X DELETE http://localhost:3000/students/1
</pre>
# License
#### This project is licensed under the MIT License. See the LICENSE file for details.

##### Feel free to explore, use, and contribute to this API. If you encounter issues or have suggestions, please open an issue or reach out to the project maintainers.




