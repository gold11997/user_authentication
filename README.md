# Node.js User Authentication - Password Login
This project demonstrates how to implement user authentication with password login using Node.js and Express. The project utilizes the bcryptjs package to securely hash passwords and verify user credentials.

## Features

- **User Registration:** Allows users to register by providing a name and password.
- **Password Hashing:** Utilizes bcrypt to securely hash and store user passwords.
- **User Login:** Validates user credentials during the login process.

## Installation

1. **Clone the repository:**

   ```bash
   git clone https://github.com/your-username/node-authentication.git

### Install dependencies:
npm install

### Usage - 
1. Run the server:
node server.js
2. Use the provided REST client to interact with the API (request.rest).

### Endpoints
- GET /users: Retrieve a list of all users.
- POST /users: Register a new user.

## Project Structure
The project consists of three main files:
# Project Components

1. **`package.json`:** Defines the project's dependencies, including Express, bcryptjs, and the Rest Client extension for Visual Studio Code.

2. **`server.js`:** Contains the Express application code, including routes for user registration, login, and listing all users.

3. **`request.rest`:** Defines the REST API calls for user registration, login, and listing all users.

## User Registration
To register a new user, send a POST request to the /users endpoint with the following JSON payload:

{
  "name": "username",
  "password": "password"
}

The server will hash the password using bcryptjs and store the user information in the users array.

### User Login
To log in an existing user, send a POST request to the /users/login endpoint with the following JSON payload:

{
  "name": "username",
  "password": "password"
}

The server will retrieve the user information from the users array and compare the provided password with the hashed password using bcryptjs. If the credentials are correct, the server will respond with a success message; otherwise, it will respond with an error message.

### Listing All Users
To list all registered users, send a GET request to the /users endpoint. The server will respond with a JSON array containing all user information except for passwords.

### Running the Project
To run the project, follow these steps:

1. Install the project dependencies using npm install or yarn install.

2. Start the Express application by running node server.js in the project directory.

3. Use the Rest Client extension in Visual Studio Code to send HTTP requests as defined in request.rest.

This project provides a basic implementation of user authentication with password login using Node.js and Express. It can be further extended to include features such as password reset, email verification, and user roles.

### **Author**
- Abraham Benson
 - Email: abrahambenson90@gmail.com
