# VartaApp(Real-Time Chat App)

## 📌 Overview
This is a **real-time chat application** built using the **MERN (MongoDB, Express, React, Node.js) stack**, **Socket.IO** for real-time communication, and **Material UI** for the frontend design. Users can create accounts, log in, and chat with other users in real time.

## 🎯 Features
✅ User authentication (JWT-based)
✅ User signup and login
✅ Real-time messaging with Socket.IO
✅ One-on-one chat functionality
✅ Group chat functionality
✅ Text, images, docs and files sharing
✅ Online/offline status updates
✅ Message persistence (stored in MongoDB)
✅ Responsive UI with Material UI
✅ Typing indicators
✅ Notifications for new messages
✅ Secure password hashing (bcrypt.js)

## 🛠️ Tech Stack
**Frontend:** React, Material UI, Axios, Socket.IO Client

**Backend:** Node.js, Express.js, MongoDB, Mongoose, Socket.IO, bcrypt.js, JWT

## 🚀 Getting Started

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/your-username/real-time-chat-app.git
cd real-time-chat-app
```

### 2️⃣ Setup the Backend (Server)
#### Navigate to the `server` folder:
```bash
cd server
```
#### Install dependencies:
```bash
npm install
```
#### Configure environment variables (`.env` file in `server` directory):
```env
PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret_key
CLIENT_URL=http://localhost:3000
```
#### Start the backend server:
```bash
npm start
```

### 3️⃣ Setup the Frontend (Client)
#### Navigate to the `client` folder:
```bash
cd ../client
```
#### Install dependencies:
```bash
npm install
```
#### Configure environment variables (`.env` file in `client` directory):
```env
REACT_APP_API_URL=http://localhost:5000
REACT_APP_SOCKET_URL=http://localhost:5000
```
#### Start the frontend server:
```bash
npm start
```

## 🌐 API Endpoints
### **Auth Routes** (`/api/auth`)
- `POST /register` - Register a new user
- `POST /login` - Authenticate user & return token

### **Chat Routes** (`/api/chat`)
- `POST /create-chat` - Create a new chat
- `GET /chats` - Get all user chats

### **Message Routes** (`/api/message`)
- `POST /send` - Send a new message
- `GET /messages/:chatId` - Get all messages in a chat

## ⚡ Real-Time Events (Socket.IO)
- `connect` - Establish WebSocket connection
- `newMessage` - Send & receive new messages
- `userTyping` - Broadcast typing indicator
- `disconnect` - Handle user disconnection

## 📷 Screenshots
[![Screenshot](https://github.com/nrmlpl/Varta-App/issues/1)]

## 🚀 Deployment
### **Backend (Server) Deployment**
Deploy the server using **Render, Heroku, or AWS**:

### **Frontend (Client) Deployment**
Deploy the frontend using **Vercel or Netlify**:
```bash
npm run build
```

## 🛠️ Future Enhancements
🔹 Voice & video calls
🔹 End-to-end encryption

## 🤝 Contributing
1. Fork the project
2. Create a new branch (`feature/your-feature`)
3. Commit your changes (`git commit -m 'Add some feature'`)
4. Push to the branch (`git push origin feature/your-feature`)
5. Open a Pull Request


## 🙌 Acknowledgments
- **MERN Stack** - MongoDB, Express, React, Node.js
- **Socket.IO** - Real-time WebSockets
- **Material UI** - UI Components
- **bcrypt.js & JWT** - Secure authentication

