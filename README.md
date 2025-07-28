# MERN Auth App 🔐

A complete **Login/Signup Authentication System** built using the **MERN Stack** (MongoDB, Express.js, React.js, Node.js). This project features secure user registration and login functionality with **JWT token-based authentication** and **password hashing** using `bcryptjs`.

---

## 📁 Tech Stack

- **MongoDB** – Database
- **Express.js** – Backend framework
- **React.js** – Frontend framework
- **Node.js** – Runtime environment
- **JWT (JSON Web Token)** – For authentication
- **bcryptjs** – For password hashing
- **dotenv** – To manage environment variables
- **CORS & axios** – For API requests

---

## 🚀 Features

- User registration
- Secure login with JWT
- Passwords hashed using `bcryptjs`
- Environment variables handled via `.env`
- Fully functional API using Express
- Frontend built with React
- Protected routes using tokens

---

## 📦 Folder Structure

MERN_login_signup/
├── backend/
│ ├── config/
│ ├── controllers/
│ ├── models/
│ ├── routes/
│ ├── .env ← [Not pushed to GitHub]
│ ├── server.js
│ └── package.json
├── frontend/
│ ├── src/
│ │ ├── components/
│ │ ├── pages/
│ │ ├── App.js
│ │ └── index.js
│ ├── public/
│ └── package.json
└── README.md

yaml
Copy
Edit

---
---

## 🔧 Installation & Setup

### 1️⃣ Backend Setup

cd backend
npm install
Create a .env file inside the backend/ folder:

env
Copy
Edit
PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_secret_key
Start the backend server:

bash
Copy
Edit
npm run dev
2️⃣ Frontend Setup
bash
Copy
Edit
cd frontend
npm install
npm start
🔐 API Routes (Backend)
Route	Method	Description
/api/auth/signup	POST	Register new user
/api/auth/login	POST	Login existing user
/api/auth/me	GET	Get logged in user (protected)

🙅‍♂️ .gitignore Setup
Make sure your .env file is NOT pushed to GitHub. Add this to .gitignore:

bash
Copy
Edit
# Ignore env file
backend/.env
If you've accidentally added it once:

bash
Copy
Edit
git rm --cached backend/.env
git commit -m "Remove .env from tracking"
git push
