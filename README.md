# Excel-analytics-platform

# 📊 Excel Analytics Platform – Backend

This is the **backend** for the Excel Analytics Platform, a full-stack MERN application where users can upload Excel files, generate 2D/3D charts, download visualizations, and get smart insights (AI optional). The backend is built using **Node.js**, **Express**, and **MongoDB Atlas**.

---

## 🚀 Features

- ✅ JWT-based authentication (User/Admin)
- ✅ Excel file uploads and parsing (using SheetJS)
- ✅ MongoDB Atlas integration
- ✅ User role management
- ✅ RESTful API structure
- ✅ Middleware for protected routes

---

## 🏗 Tech Stack

- **Node.js**
- **Express**
- **MongoDB Atlas (Mongoose)**
- **JWT for authentication**
- **Multer** (for future file uploads)
- **SheetJS (xlsx)** (for Excel parsing - future step)
- **dotenv** for environment variables

---

## 📁 Folder Structure

```
/excel-analytics-backend/src
├── controllers/          # Route logic
│   └── authController.js
├── models/               # Mongoose schemas
│   └── User.js
├── routes/               # Express route definitions
│   └── authRoutes.js
├── middleware/           # JWT and other middlewares
│   └── authMiddleware.js
├── config/
│   └── db.js             # MongoDB Atlas connection
├── .env                  # Environment variables (not committed)
├── app.js                # Express app instance
├── server.js             # App entry point
├── .gitignore
└── package.json
```

---

## 🔧 Setup Instructions

### 1. Clone the repository

```bash
git clone https://github.com/your-username/excel-analytics-backend.git
cd excel-analytics-backend
```

### 2. Install dependencies

```bash
npm install
```

### 3. Set up environment variables

Create a `.env` file in the root directory:

```env
PORT=5000
MONGO_URI=your_mongodb_atlas_connection_string
JWT_SECRET=your_secret_key
```

### 4. Run the development server

```bash
npm run dev
```

> Uses **nodemon** for auto-reload during development.

---

## 🔐 API Endpoints

| Method | Endpoint         | Description             | Access  |
| ------ | ---------------- | ----------------------- | ------- |
| POST   | /api/auth/signup | Register new user       | Public  |
| POST   | /api/auth/login  | Login user/admin        | Public  |
| GET    | /api/protected   | Example protected route | Private |

> More endpoints will be added as the project progresses.

---

## 🌍 Deployment Plan

- Backend will be deployed on **Render**
- MongoDB Atlas used for cloud-hosted database

---

## 📦 Scripts

```bash
npm start       # Run in production
npm run dev     # Run in development (with nodemon)
```

---

## 📌 Future Additions

- Excel file upload & parsing
- Chart generation APIs
- History tracking
- Admin analytics dashboard
- AI-powered data summary (OpenAI API)

---

## 👥 Contributors

- Backend Team: [Your Team Members’ Names Here]
- Project Manager: [Name if any]
