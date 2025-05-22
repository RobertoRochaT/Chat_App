# Chat Application MERN-Stack Web Application.

---

## Overview

This document provides a comprehensive overview of the Chat_App repository, a real-time messaging application built using the MERN stack (MongoDB, Express.js, React, Node.js). This overview introduces the system's architecture, technology stack, core features, and code organization to help developers understand the project structure and implementation approach.

For detailed setup instructions, see Getting Started. For specific technical implementations, refer to Frontend Application, Backend API Server, Authentication System, and Chat Features.

## System Architecture

The Chat_App follows a three-tier architecture with clear separation between presentation, business logic, and data layers. The system supports real-time communication through WebSocket connections and provides both internal JWT authentication and external provider integration.

High-Level System Architecture

## Code Organization Architecture
<img width="1141" alt="Captura de pantalla 2025-05-22 a la(s) 2 33 20 p m" src="https://github.com/user-attachments/assets/0601b59a-e741-423c-8189-fb28bac0faaf" />

## Technology Stack

| Component               | Technology            | Purpose                                 |
| ----------------------- | --------------------- | --------------------------------------- |
| Frontend Framework      | React.js              | Component-based UI development          |
| State Management        | Redux                 | Predictable application state container |
| Styling                 | Tailwind CSS          | Utility-first CSS framework             |
| Backend Framework       | Express.js            | RESTful API server                      |
| Runtime                 | Node.js               | JavaScript server environment           |
| Database                | MongoDB               | NoSQL document database                 |
| ODM                     | Mongoose              | MongoDB object modeling                 |
| Real-time Communication | Socket.IO             | Bidirectional event-based communication |
| Authentication          | JWT (JSON Web Tokens) | Secure token-based authentication       |
| Notifications           | React-Toastify        | Toast notification system               |
| Build Tool              | Vite                  | Fast frontend build tool                |

## Key Features 

The Chat-App provides comprehensive messaging functionality with the following core features:

### Authentication & User Management
- User registration and login with email/password
- JWT-based session management
- External authentication provider support (Champa-Facil API)
- Secure logout functionality

### Real-time Messaging
- Instant message delivery using Socket.IO
- One-on-one private conversations
- Group chat creation and management
- Typing indicators for active conversations
- Message read receipts and status tracking

### User Experience
- Responsive design optimized for desktop and mobile
- Toast notifications for new messages
- Sound alerts for incoming messages
- Redux-powered state management for smooth UI interactions
- Loading states and shimmer effects

## How to Install

Follow these steps to set up and run the project locally:

1.  **Clone the Repository:**

    ```bash
    git clone https://github.com/RobertoRochaT/Chat_App.git
    cd Chat_App
    ```

2.  **Install Dependencies:**
    Frontend Folder :

    ```bash
    cd frontend
    npm install
    ```

    Backend Folder :

    ```bash
    cd backend
    npm install
    ```

3.  **Set Up Environment Variables:**

    Configure the following environment variables by creating a .env file in the root of Forntend and Backend Folder:

    Frontend Folder (frontend/.env):

    ```bash
    VITE_BACKEND_URL=http://localhost:9000
    ```

    Backend Folder (backend/.env):

    ```bash
    FRONTEND_URL=http://localhost:5173
    MONGODB_URI=mongodb://127.0.0.1:27017/chat-app
    PORT=9000
    JWT_SECRET=secret-kvndkvdlkajkhkJkBiu6JJNjkbhkvnskcmhLJ5dKbkjsamnv
    ```

    Replace the values with your specific configurations.

4.  **Run the Application:**

    Frontend Folder :

    ```bash
    npm run dev
    ```

    Backend Folder :

    ```bash
    npm run dev
    ```
5.  **Development Workflow**

The application uses a dual-server development setup:
- Frontend development server runs on port `5173` using Vite
- Backend API server on port `9000` using Express.js
- MongoDB database connection on default port `27017`
  
6.  **Open in Your Browser:**

Open `http://localhost:5173` in your web browser.

## Project Structure

    ├── frontend
    │   ├── public
    │   ├── src
    │   │   ├── assets
    │   │   ├── components
    │   │   ├── pages
    │   │   ├── redux
    │   │   ├── socket
    │   │   ├── utils
    │   │   ├── App.jsx
    │   │   ├── main.jsx
    │   │   └── index.css
    │   ├── index.html
    │   ├── tailwind.config.js
    │   ├── .env
    │   └── package.json
    ├── backend
    │   ├── config
    │   ├── controllers
    │   ├── middlewares
    │   ├── models
    │   ├── routes
    │   ├── server.js
    │   ├── .env
    │   └── package.json
    └── README.md

## Author

Carlos Roberto Rocha Trejo \
Email: rochatrejocarlosroberto@gmail.com \
LinkedIn : https://www.linkedin.com/in/carlosr-rocha/


## Thank You

Thank you for exploring Chat App! Your feedback is valuable. If you have any suggestions or thoughts, feel free to share them with us. 😊

---
