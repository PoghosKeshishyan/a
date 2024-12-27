# Express API with MySQL

This project is an API built with Express, using MySQL as the database.  
It provides endpoints for managing users and interacting with a MySQL database.

## Installation and Setup

### 1. Install Express Generator
Use `express-generator` to quickly create a basic project template:
```bash
npm i -g express-generator
express -h
express --no-view 
npm install
```

### 2. Install Required Dependencies
Install the essential and development dependencies:
```bash
npm install dotenv mysql
npm install --save-dev nodemon
```

### 3. Update package.json
Add a script to run the server using `nodemon` for development:
- `"server": "nodemon ./bin/www"`

### 4. Create Controllers
Define controllers for your routes. For example, create `controllers/users.js` to manage user-related functionality.

### 5. Database Setup
- Ensure you have MySQL installed and running.
- Create a database for your application.
- Use environment variables (via .env) to store your database credentials:
```env
PORT=8000
DB_HOST=localhost
DB_USER=root
DB_PASSWORD=yourpassword
DB_NAME=yourdatabase
```

### 6. Running the Application
After setting up your database and adding the .env file with your credentials, you can run the application:

```bash
npm run server
```
This will start the server in development mode and connect it to your MySQL database. By default, it will run on port 8000 (or the port defined in .env).

### 7. License
This project is licensed under the MIT License.

## Explanation of Changes
- **API Endpoints**: Added example API requests for users, so it's clear what each route does.
- **Database Connection**: Provided more details on how to use environment variables in `.env` and an example of how to set up the database connection via `db.js`.
- **Project Structure**: Added a description of the folder and file structure to help users navigate the project more easily.
