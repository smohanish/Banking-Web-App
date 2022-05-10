# Banking-Web-App
Banking web application with basic features.

This is a Banking application made for Task 1 of GRIP(Graduate Rotational Internship Program) under The Sparks Foundation.

This Full Stack application is made using

1)Postgres SQL

2)ExpressJS

3)ReactJS

4)NodeJS

The project is hosted using heroku, here.

Checkout this same project made using Firebase and the backend on github here hosted using firebase here

Screenshots:
![image](https://user-images.githubusercontent.com/80351162/167658719-64966d3c-8b5a-49b0-a60a-8a40132a77b0.png)
![image](https://user-images.githubusercontent.com/80351162/167658814-40cd5eab-2e6c-4da3-8b52-89fa09b8c3cc.png)
![image](https://user-images.githubusercontent.com/80351162/167658859-8f37378c-426a-4d43-958d-4c611b2039e9.png)
![image](https://user-images.githubusercontent.com/80351162/167658916-86419c18-e0e6-48d0-a333-2e7000ad6819.png)


home customers transfer history

To run on your local machine:

Set up the database:

Install PostgreSQL.

create a new database.

CREATE DATABASE bank;

create new tables in that database.

CREATE TABLE customers(

    c_id SERIAL PRIMARY KEY,

    name VARCHAR(255),

    email VARCHAR(255),

    balance FLOAT

);

CREATE TABLE transfers(

    t_id SERIAL PRIMARY KEY,

    sender VARCHAR(255),

    receiver VARCHAR(255),

    transfer_amount FLOAT

);

Add mock data to the customers table.

create a .env file in the source folder of the project with the following enviornment variables.

PG_USER = postgres

PG_PASSWORD = <password of the postgres user>

PG_HOST = localhost

PG_PORT = 5432

PG_DATABASE = bank

run npm install in the root folder as well as the frontend folder.

run node index in the root folder to start the backend on http://localhost:5000.

run npm start in the frontend folder to start the react frontend at http://localhost:3000.
