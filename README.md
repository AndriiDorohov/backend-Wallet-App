<p align="center">
    <a href="https://github.com/AndriiDorohov" target="_blank">
        <img src="https://github.com/AndriiDorohov/backend-Wallet-App/blob/main/images/project-logo.png" height="100px">
    </a>
    <h1 align="center">Wallet Backend</h1>
    <br>
</p>

## _The Foundation of My Wallet Application_

[![Powered by Node.js, Express, and Swagger](https://img.shields.io/badge/Powered%20by-Node.js%2C%20Express%2C%20%26%20Swagger-%23339933)](https://github.com/AndriiDorohov/backend-Wallet-App)

[![Build Status](https://travis-ci.org/joemccann/dillinger.svg?branch=master)](https://travis-ci.org/joemccann/dillinger)

Wallet Backend is a robust and secure server-side component that serves as the backbone for my
Wallet application. It provides a reliable foundation for managing user finances efficiently.

## Frontend Repository

The Wallet Backend serves as the backbone for the Wallet Frontend. Explore the
[Wallet Frontend repository](https://github.com/AndriiDorohov/Wallet-react-app) to check out the
dynamic and user-friendly client-side application.

## DIRECTORY STRUCTURE

      db/                 contains database-related files
      docs/               contains project documentation
      logs.log            contains logs generated during runtime
      middlewares/        contains middleware files
      models/             contains model classes
      controllers/        contains controller classes
      routes/             contains route definitions
      utils/              contains utility files
      .env.example        example file for environment variables
      app.js              entry script for the application
      README.md           project documentation

## API Endpoints 🚀

### Users

| Method   | Endpoint          | Description                                      |
| -------- | ----------------- | ------------------------------------------------ |
| **POST** | `/users/register` | Register a new user.                             |
| **POST** | `/users/login`    | Log in an existing user.                         |
| **POST** | `/users/refresh`  | Refresh Tokens - requires a valid refresh token. |
| **GET**  | `/users/profile`  | Get profile of authenticated user.               |
| **GET**  | `/users/logout`   | Logout authenticated user.                       |

### Transactions

| Method     | Endpoint                                  | Description                                             |
| ---------- | ----------------------------------------- | ------------------------------------------------------- |
| **GET**    | `/transactions`                           | Get all transactions for the authenticated user.        |
| **POST**   | `/transactions`                           | Create a new transaction.                               |
| **DELETE** | `/transactions/{id}`                      | Delete a transaction by ID.                             |
| **PATCH**  | `/transactions/{id}`                      | Update a transaction by ID.                             |
| **GET**    | `/transactions/{month}/{year}`            | Filter transactions by month and year.                  |
| **GET**    | `/transactions/categories/totals`         | Get totals and sum per category.                        |
| **GET**    | `/transactions/categories/{month}/{year}` | Get totals and sum per category for a given month/year. |

### Authentication 🔑

The API uses JWT tokens for authentication. Register and login endpoints provide new tokens. Provide
the Bearer token in the Authorization header to authenticate requests.

### Error Handling

- Validation errors return a 400 status with a ValidationError response.
- Unauthorized requests return a 401 status.
- NotFound errors return a 404 status.
- Other server errors return a 500 status.

## Tech

The "Wallet Backend" project leverages a variety of open-source technologies:

- [Node.js] - event-driven I/O for the backend
- [Express] - fast framework for building network applications on Node.js
- [Swagger] - tool for creating interactive API documentation
- [Mongoose] - library for modeling objects for MongoDB and Node.js
- [Axios] - HTTP client for making requests
- [Cors] - package for handling CORS requests in Express
- [jsonwebtoken] - library for generating and verifying JWT tokens
- [bcryptjs] - library for hashing passwords
- [dotenv] - module for loading environment variables from a .env file
- [log4js] - library for event logging in Node.js
- [moment] - library for working with dates and times in JavaScript
- [uuid] - generator for unique identifiers
- [validator] - library for data validation

And, of course, the "Wallet Backend" itself is an open-source project with a public repository on
GitHub.

## Installation

For running the "Wallet Backend," you need [Node.js](https://nodejs.org/) v12+ installed on your
system.

Clone the repository

```sh
git clone https://github.com/AndriiDorohov/backend-Wallet-App.git
```

Navigate to the project directory

```sh
cd backend-Wallet-App
```

Install dependencies

```sh
npm install
```

Start the development server

```sh
npm run start:dev
```

##### For production environments

Install production dependencies

```sh
npm install --production
```

Set the environment to production and start the server

```sh
NODE_ENV=production npm start
```

## License

MIT

**Free Software, Hell Yeah!**
