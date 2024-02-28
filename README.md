Permalist - An advanced To Do List that has all four main operation of the Datbase i.e. CRUD (Create Read Update Delete) .
To run this :-
1. Download (https://github.com/Gaurav-Sharma-2002/To-Do-List_advanced/archive/refs/heads/main.zip) -> Extract -> Open the extracted folder inside VS Code .

2. Open terminal , cd into Project folder .

3. Run npm i , to install all the required dependencies .

4. Setup your SQL database with following queries :
i) CREATE TABLE items (
  id SERIAL PRIMARY KEY,
  title VARCHAR(100) NOT NULL
);
, to create the required database that supports this project (I'm using PostgreSQL 15, Pgadmin 4) .

ii) INSERT INTO items (title) VALUES ('Buy milk'), ('Finish homework');
, creating some sample data inside the database .

5. Replace the following with your own credentials in the Index.js file :
  user: process.env.PG_USER,
  host: process.env.PG_HOST,
  database: process.env.PG_DATABASE,
  password: process.env.PG_PASSWORD,
  port: process.env.PG_PORT,

6. Then in terminal , Run node index.js , to start the application .
