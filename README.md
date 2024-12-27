# Express API with PRISMA ORM and SQLite3
This project is an API built with Express, using Prisma ORM to interact with a SQLite3 database.  
It provides endpoints for managing cars and other resources, with Prisma handling the database operations. Prisma simplifies database queries, migrations, and schema management.
With Prisma, you can easily define your database schema and interact with the SQLite3 database in a more efficient and organized manner. It offers a type-safe way to access and manage data through its generated client.


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
npm install dotenv
npm install --save-dev nodemon
```

### 3. Install PRISMA ORM
Install Prisma ORM and its required dependencies:
```bash
npm install prisma --save-dev
npx prisma init --datasource-provider sqlite
```
We modify the ՝schema.prisma՝ file and write our ՝model՝.
```bash
npx prisma migrate dev --name init
```
Create the `prisma-client.js` file in the `prisma` folder to initialize the Prisma client:


### 4. Update package.json
Add a script to run the server using `nodemon` for development:
```json
"server": "nodemon ./bin/www"
```


### 5. Create Controllers
Define controllers for your routes. For example, create `controllers/comments.js` to manage car-related functionality.


### 6. Running the Application
Before running the application, ensure you have added the following line to your `.env` file to define the port:
```env
PORT=8000
```
After setting up your database and adding the `.env` file with your credentials, you can run the application:
```bash
npm run server
```
This will start the server in development mode and connect it to your SQLite3 database. By default, it will run on `localhost:8000` (or the port defined in `.env`).


### 7. License
This project is licensed under the MIT License.