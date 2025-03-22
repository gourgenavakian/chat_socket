# 📌 Fullstack Chat Application

## 📖 Description
This is a fullstack chat application built with React, Node.js, and MongoDB, offering real-time messaging via WebSockets (Socket.io). It features user registration and authentication using JWT, image uploads, and a responsive UI styled with Bootstrap. The app supports Docker for easy deployment and containerization.

## 🛠 Technologies Used
- **Frontend:** React.js, Bootstrap
- **Backend:** Node.js, Express, MongoDB
- **WebSockets:** Socket.io
- **Authentication:** JWT
- **Deployment:** Docker

## 📂 Project Structure
```
├── docker-compose.yml        # Docker Compose configuration
├── front                    # Frontend (React)
│   ├── Dockerfile           # Docker configuration
│   ├── src
│   │   ├── components       # UI components
│   │   ├── services         # WebSocket connection
│   │   ├── assets           # Media files
│   │   ├── App.js           # Main component
│   │   ├── index.js         # Entry point
│   ├── package.json         # Dependencies
│   ├── public               # Static files
└── server                   # Backend (Node.js)
    ├── Dockerfile           # Docker configuration
    ├── app.js               # Server entry point
    ├── config               # Database connection
    ├── controllers          # Request handlers
    ├── middlewares          # Middleware files
    ├── models               # MongoDB models
    ├── routes               # API routes
    ├── sockets              # WebSockets
    ├── uploads              # File upload
    ├── package.json         # Dependencies
```

## 🚀 Installation & Setup

### 1️⃣ Clone the Repository
```bash
git clone git@github.com:gourgenavakian/chat_socket.git
cd chat_socket
```

### 2️⃣ Run with Docker
```bash
docker-compose up --build
```

### 3️⃣ Run Manually
#### Install Dependencies
```bash
cd front && npm install  # Frontend
cd ../server && npm install  # Backend
```

#### Start Backend
```bash
cd server
npm start
```

#### Start Frontend
```bash
cd front
npm start
```

## 🔗 API Endpoints
- **POST** `/api/users/register` - Register a user
- **POST** `/api/users/login` - User login
- **GET** `/api/users/profile` - Fetch user profile
- **POST** `/api/upload` - Upload image
- **GET** `/api/chats` - Get chat list



## 🔜 TODO
- [ ] Improve UI/UX with better design
- [ ] Implement push notifications for new messages
- [ ] Add typing indicators in chat
- [ ] Support for group chats
- [ ] Implement message editing and deletion
- [ ] Optimize WebSocket performance
- [ ] Add read receipts for messages
- [ ] Improve Docker setup for production deployment

## 👨‍💻 Author
**Gourgen Avakian** - [GitHub](https://github.com/gourgenavakian) | [LinkedIn](https://www.linkedin.com/in/gourgen-avakian/)

## 📄 License
This project is licensed under the MIT License.

