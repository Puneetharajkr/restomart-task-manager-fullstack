#  Restomart Task Manager - Fullstack Application (No Auth)

## Candidate: Puneetharaj K R  
## Project: Task Manager (Full Stack)  
This is a simple full-stack **Task Manager** application developed as part of the **Restomart Technical Internship Assignment**. It allows users to **add, edit, delete, and list tasks** without authentication. The application is clean, functional, and uses RESTful API design principles.

---

## Tech Stack

| Layer     | Technologies Used                         |
|-----------|-------------------------------------------|
| Backend   | Node.js, Express.js, TypeORM, SQLite      |
| Frontend  | React.js, Axios, React Router, CSS        |
| Database  | SQLite (file-based, no external setup)    |
| Deployment| Render (backend), Vercel (frontend)       |

---

## Live Demo

- **Frontend** (React):  
   [https://task-manager-frontend-puneetharaj-k-rs-projects.vercel.app/](https://task-manager-frontend-puneetharaj-k-rs-projects.vercel.app/)

- **Backend** (Express + SQLite):  
   [https://task-manager-backend-9xgx.onrender.com](https://task-manager-backend-9xgx.onrender.com)

---

## Repository Structure



restomart-task-manager-fullstack/
├── Task_Manager_Backend/ → Node.js + Express.js + SQLite
└── Task_Manager_Frontend/ → React.js + React Router + Axios + CSS



---

## Setup Instructions

### Backend Setup (`/backend`)

#### Prerequisites:
- Node.js v16+
- npm or yarn

#### Installation & Run:

cd backend
npm install          # Install dependencies
npm run dev          # Start the backend server

### SQLite Setup:
No setup required!
TypeORM will automatically create a database.sqlite file in the root on first run.

### API Base URL:
http://localhost:3001

### Sample API Endpoints:
| Method | Endpoint     | Description       |
| ------ | ------------ | ----------------- |
| GET    | /tasks       | List all tasks    |
| POST   | /tasks       | Create a new task |
| PUT    | /tasks/:id   | Update a task     |
| DELETE | /tasks/:id   | Delete a task     |


# Frontend Setup (/frontend)
### Prerequisites:
Node.js v16+
npm or yarn

### Installation & Run:
cd frontend
npm install              # Install frontend dependencies
npm start                # Run React app on localhost:3000

### Configure API URL:
Create .env file in /frontend: REACT_APP_API_URL=http://localhost:3001
     You can refer to .env.example for this structure.

# Pages Overview
| Route       | Page      | Functionality                   |
| ----------- | --------- | ------------------------------- |
| /           | Home      | List all tasks                  |
| /add        | Add Task  | Form to create a new task       |
| /edit/:id   | Edit Task | Form to update an existing task |

# Actions Supported:
Add a task
Edit a task
Delete a task

# Task Model (Backend)
| Field       | Type                           | Required | Description             |
| ----------- | ------------------------------ | -------- | ----------------------- |
| id          | UUID                           | Yes      | Primary Key             |
| title       | String                         | Yes      | Title of the task       |
| description | Text                           | No       | Task details            |
| status      | Enum: todo, in\_progress, done | Yes      | Task status             |
| dueDate     | Date                           | No       | Optional deadline       |
| createdAt   | Timestamp                      | Yes      | Auto-set by TypeORM     |
| updatedAt   | Timestamp                      | Yes      | Auto-updated by TypeORM |


# Environment Configurations
### Backend (/backend/.env.example)
PORT=3001

### Frontend (/frontend/.env.example)
REACT_APP_API_URL=http://localhost:3001

# Future Improvements
Add user authentication & authorization
Improve UI with Tailwind or design system
Add filtering by status on homepage
Implement pagination for long task lists

#  Contact
Candidate: Puneetharaj K R
GitHub: @Puneetharajkr
Email: puneetharajkr123@gmail.com

