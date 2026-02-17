# Task Manager Web Application

A simple task management web application built with Node.js, Express, MongoDB, and vanilla JavaScript.

## Features

- Create new tasks
- View all tasks
- Edit existing tasks
- Delete tasks
- Toggle task status (Pending/Completed)

## Tech Stack

**Frontend:**
- HTML
- CSS
- Vanilla JavaScript

**Backend:**
- Node.js
- Express.js
- MongoDB
- Mongoose

## Project Structure

```
task-manager/
│
├── backend/
│   ├── server.js
│   ├── models/
│   │   └── Task.js
│   ├── routes/
│   │   └── taskRoutes.js
│   └── package.json
│
├── frontend/
│   ├── index.html
│   ├── style.css
│   └── script.js
│
└── README.md
```

## Installation

### Prerequisites

- Node.js (v14 or higher)
- MongoDB (running locally or MongoDB Atlas)

### Steps

1. Clone or download this project

2. Install backend dependencies:
```bash
cd backend
npm install
```

## MongoDB Setup

### Option 1: Local MongoDB

1. Install MongoDB on your system
2. Start MongoDB service:
```bash
# On Windows
net start MongoDB

# On Mac (using Homebrew)
brew services start mongodb-community

# On Linux
sudo systemctl start mongod
```

3. The application will connect to `mongodb://localhost:27017/taskmanager`

### Option 2: MongoDB Atlas (Cloud)

1. Create a free account at [MongoDB Atlas](https://www.mongodb.com/cloud/atlas)
2. Create a new cluster
3. Get your connection string
4. Update the connection string in `backend/server.js`:
```javascript
mongoose.connect('your-mongodb-atlas-connection-string')
```

## Running the Application

### Start Backend Server

bash
cd backend
npm start


The server will run on `http://localhost:5000`

You should see: `Connected to MongoDB` and `Server running on http://localhost:5000`

