# 🧩 Flutter Mongo Backend (AI Nutrition App)

This is the backend server for the **AI Nutrition App**, built with **Node.js**, **Express**, and **MongoDB**.  
It handles user registration, login, and communication with the Flutter frontend.

---

## ⚙️ Tech Stack

- **Backend Framework:** Node.js + Express  
- **Database:** MongoDB (using Mongoose)  
- **API Type:** RESTful APIs  
- **Frontend:** Flutter mobile app  
- **Authentication:** Basic user auth (username, email, password)

---

## 📁 Project Structure

```
flutter_mongo_backend/
│
├── server.js # Main server entry point
├── models/
│   └── User.js # Mongoose User schema
├── routes/
│   └── auth.js # Register & Login routes
├── .env # Environment variables (Mongo URI, etc.)
└── package.json # Project dependencies
```

---

## 🚀 Getting Started

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/meghanag4/flutter_mongo_backend.git
cd flutter_mongo_backend
```

### 2️⃣ Install Dependencies
```bash
npm install
```

### 3️⃣ Configure Environment Variables
Create a `.env` file in the root directory:

```
MONGO_URI=mongodb://127.0.0.1:27017/ai_nutrition_app
PORT=5000
```

### 4️⃣ Run the Server
```bash
node server.js
```

If successful, you’ll see:
```
✅ Server running on port 5000
✅ Connected to MongoDB
```

---

## 🧠 API Endpoints

### 🔹 Register User
**POST** `/register`

**Body:**
```json
{
  "username": "meghana",
  "email": "meghana@gmail.com",
  "password": "123456"
}
```

**Response:**
```json
{
  "message": "User registered successfully"
}
```

---

### 🔹 Login User
**POST** `/login`

**Body:**
```json
{
  "username": "meghana",
  "password": "123456"
}
```

**Response:**
```json
{
  "message": "Login successful"
}
```

---

## 📦 Dependencies

- express  
- mongoose  
- dotenv  
- cors  
- body-parser  

Install them with:
```bash
npm install express mongoose dotenv cors body-parser
```

---

## 👩‍💻 Author
**Meghana G**

📧 GitHub: [@meghanag4](https://github.com/meghanag4)

---

## 🧾 License
This project is licensed under the **MIT License** — feel free to modify and use it.

✅ Now you can easily connect this backend with your Flutter frontend using your local IP and port (e.g., `http://<your-ip>:5000`).
