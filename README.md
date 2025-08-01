# 📚 Book Club Library Management System

<div align="center">
  <img src="https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB" alt="React" />
  <img src="https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white" alt="TypeScript" />
  <img src="https://img.shields.io/badge/Node.js-43853D?style=for-the-badge&logo=node.js&logoColor=white" alt="Node.js" />
  <img src="https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white" alt="MongoDB" />
  <img src="https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white" alt="Tailwind CSS" />
</div>

<div align="center">
  <h3>🌟 A Full-Stack Solution to Manage Books, Readers & Lending at Book Club Library </h3>
  <p>Digitally transforming library operations with modern web technologies</p>
</div>

---

## 🎯 Overview

A full-stack web application for managing books, readers, and lending transactions in a library.
Built with a **React (TypeScript)** frontend and a **Node.js/Express** backend.
---

## ✨ Key Features

- 📖 **Reader & Book Management**: Full CRUD operations
- 🔄 **Lending & Return System**: Tracks due dates and borrowing history
- ⏰ **Overdue Notifications**: Automatic email reminders
- 🔐 **Authentication**: JWT-secured access with role-based control
- 📊 **Dashboard Analytics**: Real-time insights on lending and inventory
- 📂 **Audit Logs**: Trace all actions for accountability
- 🔎 **Search & Filter**: Fast lookup across readers/books

---

## 🛠️ Technology Stack

| Layer         | Tech                             |
|--------------|----------------------------------|
| **Frontend** | React 18, TypeScript, Tailwind CSS |
| **Backend**  | Node.js, Express.js, TypeScript   |
| **Database** | MongoDB, Mongoose ODM             |
| **Security** | JWT, bcrypt                       |
| **Email**    | Nodemailer                        |
| **Tooling**  | Vite, Nodemon                     |

---

## 📁 Project Structure

```
Book-Club-Library/
├── client/          # React Frontend
│   └── src/
│       ├── components/
│       ├── context/
│       ├── pages/
│       ├── services/
│       └── router.tsx
├── server/          # Node.js Backend
│   └── src/
│       ├── controllers/
│       ├── models/
│       ├── middlewares/
│       └── routes/
├── postman/         # API Documentation
```

---

## 🚀 Quick Start

### 🧱 Prerequisites

- Node.js ≥ v16
- MongoDB (local or Atlas)
- npm / yarn

### ⚙️ Installation

```bash
# Clone the repository
git clone https://github.com/yourusername/book-club-library.git
cd book-club-library
```

#### Backend Setup

```bash
cd server
npm install

# Create a .env file
touch .env
```

Add environment variables:
```env
MONGODB_URI=mongodb://localhost:27017/book-club-library
JWT_SECRET=your-super-secret-jwt-key
EMAIL_USER=your-email@gmail.com
EMAIL_PASS=your-app-password
PORT=3000
```

Start server:
```bash
npm run dev
```

#### Frontend Setup

```bash
cd ../client
npm install
npm run dev
```

---

## 📡 API Documentation

### 🔗 Postman Collection

Import from:
[`Book_Club_Library.postman_collection.json`](postman/Book-Club-API.json)

### 🌐 Base URL

```
http://localhost:3000/api
```

### 🧾 Sample Endpoints

| Method | Endpoint                    | Description                    |
|--------|-----------------------------|--------------------------------|
| POST   | `/auth/login`               | Login for staff users          |
| GET    | `/readers`                  | View all registered members    |
| POST   | `/books`                    | Add a new book                 |
| POST   | `/lending`                  | Issue a book to a reader       |
| GET    | `/lending/overdue`          | Get list of overdue books      |

---

## 🔧 Development

### 🔁 Scripts

**Backend:**
```bash
npm run dev     # Start with nodemon
npm run build   # Compile TS
npm start       # Run production
```

**Frontend:**
```bash
npm run dev     # Start Vite dev server
npm run build   # Production build
npm run lint    # Code linting
```

### 🧹 Code Standards

- TypeScript-first development
- ESLint for linting
- Modular component & API structure

---

## 🌐 Deployment

### 🌱 Environment Variables

Ensure `.env` includes:
- MongoDB connection string
- JWT secret keys
- SMTP credentials

### ⚒️ Production Build

```bash
# Backend
cd server
npm run build
npm start

# Frontend
cd client
npm run build
```

Deploy frontend `dist/` via static hosting or reverse proxy (e.g., Nginx).

---

## 🤝 Contributing

We welcome contributions!

1. Fork the repo
2. Create your branch (`git checkout -b feature-name`)
3. Commit your changes
4. Push and create a PR

---

## 📄 License

This project is licensed under the **MIT License** – see the [LICENSE](LICENSE) file for details.

---

## 👨‍💻 Author

**Thanura Vipulanga**  
- GitHub: [@Thanu-2002](https://github.com/Thanu-2002)  
- Email: thanuravipulanga2000@gmail.com

---

<div align="center">
  <strong>📚 Made with care for Book Club Library</strong><br />
  <small>© 2025 Book Club Library System. All rights reserved.</small>
</div>
