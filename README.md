# Permalist - An Advanced To-Do List Application

Permalist is an advanced to-do list application that supports all four main database operations: CRUD (Create, Read, Update, Delete).

## Getting Started

To run this application, follow these steps:

1. **Download and Extract**
   - Download the source code from [this link](https://github.com/Gaurav-Sharma-2002/To-Do-List_advanced/archive/refs/heads/main.zip).
   - Extract the downloaded file.
   - Open the extracted folder in your favorite code editor such as Visual Studio Code.

2. **Install Dependencies**
   - Open a terminal.
   - Navigate to the project folder using `cd`.
   - Run `npm install` to install all the required dependencies.

3. **Setup SQL Database**
   - Set up your SQL database ( I'm using PostgreSQL (version 15) and PgAdmin 4 ) .
   - Execute the following SQL queries to create the required database table and insert sample data:

```sql
CREATE TABLE items (
  id SERIAL PRIMARY KEY,
  title VARCHAR(100) NOT NULL
);

INSERT INTO items (title) VALUES ('Buy milk'), ('Finish homework');
```
4. **Replace Database Credentials**
    - Open the index.js file.
    - Replace the following database connection credentials with your own :
```
   user: process.env.PG_USER,
   host: process.env.PG_HOST,
   database: process.env.PG_DATABASE,
   password: process.env.PG_PASSWORD,
   port: process.env.PG_PORT,
```
5. **Run the Application**
   - In the terminal, run node index.js to start the application.
