# Backend Template with React JS and Flask API

Build web applications using React.js for the frontend and Python/Flask for your backend API.

- Documentation can be found here: https://start.4geeksacademy.com/starters/react-flask  
- Here is a video on [how to use this template](https://www.loom.com/share/f37c6838b3f1496c95111e515e83dd9b)  
- Integrated with Pipenv for backend package management and npm/yarn for frontend dependencies.  
- Fast deployment to Heroku and Render.  
- Use of `.env` file for environment variables.  
- SQLAlchemy integration for database ORM.

---

### 1) Backend Installation

If you use Github Codespaces (recommended) or Gitpod, this template will already have Python, Node.js, and PostgreSQL installed. If you are working locally, make sure you have installed:

- Python 3.8 or higher  
- Pipenv  
- A database engine (PostgreSQL recommended)

Steps:

1. Install the Python packages:

```bash
pipenv install
Create a .env file based on .env.example:

bash
Copiar
Editar
cp .env.example .env
Install and configure your database engine. Set the DATABASE_URL environment variable accordingly in .env:

Engine	DATABASE_URL
SQLite	sqlite:////test.db
MySQL	mysql://username:password@localhost:port/example
PostgreSQL	postgres://username:password@localhost:5432/example

Run the migrations to create tables:

bash
Copiar
Editar
pipenv run migrate
pipenv run upgrade
Start the backend application:

bash
Copiar
Editar
pipenv run start
Note: Codespaces users can connect to psql by running:
psql -h localhost -U gitpod example

Undo a migration
You can undo a migration by running:

bash
Copiar
Editar
pipenv run downgrade
Backend: Populate Users Table
To insert test users into the database, run:

bash
Copiar
Editar
flask insert-test-users 5
Expected output:

nginx
Copiar
Editar
Creating test users
test_user1@test.com created.
test_user2@test.com created.
test_user3@test.com created.
test_user4@test.com created.
test_user5@test.com created.
Users created successfully!
To automate adding more test data, edit the insert_test_data function in src/api/commands.py.

2) Frontend Manual Installation
Make sure you are using Node.js version 14 or higher, and that the backend is already installed and running.

Install the frontend packages:

bash
Copiar
Editar
npm install
Start the frontend development server:

bash
Copiar
Editar
npm run start
Deploy your website!
This boilerplate is ready to deploy with Render.com and Heroku in minutes. Please check the official deployment documentation for details.

Contributors
This template was built as part of the 4Geeks Academy Coding Bootcamp by Alejandro Sanchez and many other contributors.

Learn more about our Full Stack Developer Course, and Data Science Bootcamp.

Find more templates and resources at the 4Geeks Academy GitHub page.
