# MySQL Express

A CRUD app built with Node.js, Express, and MySQL. It generates fake users with Faker and lets you view, edit, and delete them through EJS pages.

## Features
- Connects Express to a MySQL database (`mysql2`)
- Generates and inserts fake user data (`@faker-js/faker`)
- Edit and delete users using `method-override`
- Server-side pages with EJS (`views/`)

## Tech
Node.js, Express, MySQL, EJS

## Requirements
- Node.js
- MySQL running locally, with a database named `delta_app`
- Tables created from `schema.sql`

## Setup

1. Install packages:

        npm install

2. Create a `.env` file in the project folder (see `.env.example`):

        DB_PASSWORD=your-mysql-password

3. Create the database and tables in MySQL:

        CREATE DATABASE delta_app;

   Then run the SQL in `schema.sql`.

4. Start the app:

        node index.js

5. Open http://localhost:8080

The app connects as user `root` on `localhost`. Change these values in `index.js` if your MySQL setup is different.

## Author
Muhammad Hilal