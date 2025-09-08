# Authentication API

A simple Node.js + Express + MySQL authentication API.  
This project demonstrates how to set up a RESTful backend with user authentication features.

---

## 🚀 Project Overview
This project provides a backend API for authentication, including:
- User registration
- User login
- Health check endpoint
- Database connection with MySQL

Built with:
- [Node.js](https://nodejs.org/)
- [Express](https://expressjs.com/)
- [MySQL2](https://www.npmjs.com/package/mysql2)
- [dotenv](https://www.npmjs.com/package/dotenv)
- [CORS](https://www.npmjs.com/package/cors)

---

## ⚙️ Setup

1. Clone the repository
   git clone https://github.com/your-username/your-repo.git
   cd your-repo
2. Install dependencies
    npm install
3. Configure environment variables
    (Create a .env file in the project root and add:)
    SERVER_PORT=3000
    DB_HOST=localhost
    DB_USER=root
    DB_PASS=
    DB_NAME=lab_auth
    DB_PORT=3306
4. Set up MySQL database
    Create a database named lab_auth (or your chosen name).

    Run your migration/SQL schema to create the required tables.

## 📡 API Endpoints
Health Check
    GET /api/health
    Returns server and database status.

Authentication
    POST /api/register
    Register a new user.
    Body (JSON):
        {
        "username": "testuser",
        "password": "secret123"
        }

    POST /api/login
    Authenticate a user and return a token/session.
    Body (JSON):
        {
        "username": "testuser",
        "password": "secret123"
        }
## Other Notes:
    >Ensure MySQL and Apache is running before starting the server.
    >Use a tool like Postman to test the endpoints.
