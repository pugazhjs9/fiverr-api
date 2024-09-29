# Fiverr API Backend

This is a backend project built using **Node.js**, **Express**, and **Prisma ORM** with **MySQL** for handling user authentication, including signup and login functionalities.

## Features

- User signup and login.
- JWT-based authentication.
- Prisma ORM integration with MySQL.
- CORS enabled for frontend requests.

## Installation

1. **Clone the repository:**

   ```bash
   git clone <repo-url>
   ```

2. **Install dependencies:**

   ```bash
   npm install
   ```

3. **Set up Prisma:**

   - Update the `schema.prisma` file with your MySQL connection details.
   - Run Prisma migrations:

     ```bash
     npx prisma migrate dev
     ```

4. **Start the server:**

   ```bash
   npm start
   ```

   The backend server will run on port **8801**.

## API Endpoints

- **Signup:**
  - `POST /signup`
  - Body: `{ email: string, password: string }`
  - Creates a new user if not already registered.

- **Login:**
  - `POST /login`
  - Body: `{ email: string, password: string }`
  - Authenticates the user and returns a JWT token.

## Technologies Used

- **Node.js**
- **Express.js**
- **Prisma ORM**
- **MySQL**
- **JWT for authentication**
- 
