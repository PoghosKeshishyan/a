# Express API with MySQL

This project is an API built with Express, using MySQL as the database.

## Installation and Setup

### 1. Install Express Generator
Use `express-generator` to quickly create a basic project template:
```bash
npm i -g express-generator
express -h
express --no-view 
```

### 2. Install Required Dependencies
Install the essential and development dependencies:

`npm install dotenv mysql`
`npm install --save-dev nodemon`


### 3. Update package.json
Add a script to run the server using nodemon:

`"server": "nodemon ./bin/www"`

Run the server in development mode:
`npm run server`


### 4. Create Controllers
Define controllers for the routes. For example:

controllers/users.js


### 5. Database Setup
Ensure you have MySQL installed and running.
Create a database for your application.
Use environment variables (via .env) to store your database credentials:

`DB_HOST=localhost`
`DB_USER=root`
`DB_PASSWORD=yourpassword`
`DB_NAME=yourdatabase`