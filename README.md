# Family-Travel-Tracker
A web app to track visited countries and manage family members with custom colors. Built with Node.js, Express, and PostgreSQL.

Prerequisites
Before you begin, ensure that you have the following installed on your system:

Node.js: JavaScript runtime.
PostgreSQL: Database server.

1. Install Dependencies
Install the required dependencies using npm:
npm install

2. Set Up PostgreSQL Database
You need to create a PostgreSQL database and tables for the application.

a. Create Database
Log in to PostgreSQL and create a new database (e.g., world):
b. Create Tables
Run the following SQL commands to create the necessary tables (users, countries, visited_countries):provided in the queries.sql
c. Populate countries Table
You may populate the countries table with country names and their corresponding codes. You can either manually insert data or import a dataset of countries from countries.csv

3. Add PostgreSQL Credentials
In the index.js file, update the PostgreSQL connection credentials to match your local database settings. Locate this section in your code:

const db = new pg.Client({
  user: "postgres",        // Your PostgreSQL username
  host: "localhost",
  database: "world",       // Your database name
  password: "123456",      // Your PostgreSQL password
  port: 5432,
});
Replace the user, database, and password with your own PostgreSQL credentials.

4. Run the Application
To start the application, run the following command:node index.js

5. Access the Application



Open your browser and go to http://localhost:3000.
You can add new users, select a favorite color, and start adding visited countries.
6. SCREENSHOTS OF THE PROJECT:
![Screenshot 2025-04-27 202446](https://github.com/user-attachments/assets/ec0004ae-9909-434b-9fa6-d3ac2a065f43)
![Screenshot 2025-04-27 202414](https://github.com/user-attachments/assets/07506372-d154-4a58-aa84-e7dcdae0ac45)



