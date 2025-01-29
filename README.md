# SACE Backend

This is the backend for the SACE project, built using the MERN stack (MongoDB, Express, React, Node.js). It includes user authentication, project management, and AI integration.

## Prerequisites

- Node.js
- MongoDB
- Redis
- Web Containers

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/ManavKaneriya37/SACE.git
    cd SACE/Backend
    ```

2. Install dependencies:
    ```bash
    npm install
    ```


## Running the Server

1. Start the server:
    ```bash
    node server.js
    ```

## API Endpoints

### User Routes

- `POST /users/signup` - Sign up a new user
- `POST /users/signin` - Sign in an existing user
- `GET /users/profile` - Get the profile of the logged-in user
- `POST /users/logout` - Log out the current user
- `GET /users` - Get all users except the logged-in user

### Project Routes

- `POST /projects` - Create a new project
- `GET /projects` - Get all projects of the logged-in user
- `POST /projects/addUser` - Add users to a project
- `GET /projects/:projectId` - Get a project by ID
- `PUT /projects/updateFileTree` - Update the file tree of a project

### AI Routes

- `POST /ai/result` - Get AI-generated result based on a prompt

## Directory Structure

```
Backend/
├── controllers/
│   ├── ai.controller.js
│   ├── project.controller.js
│   └── user.controller.js
├── database/
│   └── dbConnection.js
├── models/
│   └── user.model.js
├── routes/
│   ├── ai.routes.js
│   ├── project.routes.js
│   └── user.routes.js
├── services/
│   ├── ai.service.js
│   ├── project.service.js
│   ├── redis.service.js
│   └── user.service.js
├── .env
├── .gitignore
├── app.js
├── package.json
├── package-lock.json
└── server.js
```

# SACE Frontend

This is the frontend for the SACE project, built using React. It includes user authentication, project management, and AI integration.


## Installation

1. Install dependencies:
    ```bash
    npm install
    ```

## Running the Application

1. Start the development server:
    ```bash
    npm run dev
    ```

## Directory Structure

```
Frontend/
├── public/
│   ├── index.html
│   └── ...
├── src/
│   ├── components/
│   │   ├── Auth/
│   │   │   ├── SignIn.js
│   │   │   └── SignUp.js
│   │   ├── Project/
│   │   │   ├── ProjectList.js
│   │   │   └── ProjectDetails.js
│   │   ├── AI/
│   │   │   └── AIResult.js
│   │   └── ...
│   ├── context/
│   │   ├── AuthContext.js
│   │   └── ProjectContext.js
│   ├── services/
│   │   ├── api.js
│   │   └── auth.js
│   ├── App.js
│   ├── index.js
│   └── ...
├── .env
├── .gitignore
├── package.json
└── package-lock.json
```
