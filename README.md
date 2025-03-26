# To-Do List Application

This repository contains both the frontend and backend for a To-Do List application.

## Features
- User authentication (JWT/OAuth)
- Create, read, update, and delete (CRUD) tasks
- Secure API with Express and MongoDB
- Interactive UI built with React

## Prerequisites
Ensure you have the following installed:
- [Node.js](https://nodejs.org/) (v16+ recommended)
- [MongoDB](https://www.mongodb.com/) (local or cloud-based like MongoDB Atlas)
- [Git](https://git-scm.com/)

## Installation

### 1. Clone the Repository
```sh
git clone https://github.com/AbhishekRatho-2004/Task-01-Todo-List.git
cd Task-01-Todo-List
```

### 2. Backend Setup
Navigate to the backend directory and install dependencies:
```sh
cd backend
npm install
```

#### Configure Environment Variables
Create a `.env` file in the `backend` directory and add:
```
PORT=5000
MONGO_URI=your_mongodb_connection_string
```

#### Start Backend Server
```sh
nodemon index.js
```
The backend server will run at `http://localhost:5000`

### 3. Frontend Setup
Navigate to the frontend directory and install dependencies:
```sh
cd ../frontend
npm install
```

#### Start Frontend Server
```sh
npm run dev
```
The frontend will run at `http://localhost:5173`

## Running Both Together
You can run both the frontend and backend simultaneously using **concurrently**:
```sh
cd Task-01-Todo-List
npm install -g concurrently
concurrently "cd backend && npm start" "cd frontend && npm start"
```

## API Endpoints

### Tasks
- `POST /api/tasks` – Create a new task
- `GET /api/tasks` – Get all tasks
- `PUT /api/tasks/:id` – Update a task
- `DELETE /api/tasks/:id` – Delete a task

## Technologies Used
- **Backend**: Node.js, Express, MongoDB, Mongoose
- **Frontend**: React, Axios, MUI


