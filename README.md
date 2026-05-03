# Team Task Manager

A modern, full-stack task management application designed for teams to collaborate efficiently. Built with the MERN stack and deployed on Railway.
---

## Features

- **Authentication**: Secure login and signup using JWT and Bcrypt.
- **Task Management**: Create, update, delete, and track tasks.
- **Team Collaboration**: Assign tasks to team members.
- **Responsive Design**: Fully optimized for all device sizes.
- **Real-time Updates**: Instant feedback on task status changes.

## Tech Stack

### Frontend
- **Framework**: React 19 (Vite)
- **Routing**: React Router 7
- **HTTP Client**: Axios
- **State Management**: React Hooks

### Backend
- **Runtime**: Node.js
- **Framework**: Express
- **Database**: MongoDB (via Mongoose)
- **Security**: JWT & Bcrypt

---

## Getting Started

Follow these steps to set up the project locally.

### Prerequisites
- Node.js (v18 or higher)
- MongoDB account or local instance

### 1. Clone the Repository
```bash
git clone <repository-url>
cd team-task-manager
```

### 2. Backend Setup
```bash
cd backend
npm install
```
Create a `.env` file in the `backend` directory and add the following:
```env
PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_secret_key
```
Run the backend server:
```bash
npm run dev
```

### 3. Frontend Setup
```bash
cd ../frontend
npm install
```
Start the frontend development server:
```bash
npm run dev
```

---

## Deployment (Railway)

This project is configured for deployment on railway

### Steps to Deploy:
1. **Connect GitHub**: Link your repository to a new Railway project.
2. **Add Services**:
   - Create two services: one for the **Backend** and one for the **Frontend**.
   - Set the **Root Directory** for each service accordingly (`/backend` and `/frontend`).
3. **Environment Variables**:
   - For the Backend service, add the following variables in the Railway dashboard:
     - `PORT`: `5000` (or your preferred port)
     - `MONGO_URI`: Your MongoDB Atlas connection string.
     - `JWT_SECRET`: A strong secret key.
4. **Build & Deploy**: Railway will automatically detect the `package.json` files and build the services using Nixpacks.

---

## Environment Variables

| Variable | Description | Default |
|----------|-------------|---------|
| `PORT` | Port number for the backend server | `5000` |
| `MONGO_URI` | MongoDB connection string | - |
| `JWT_SECRET` | Secret key for JWT authentication | - |

Made by Aryan kumar
