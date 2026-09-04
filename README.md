# MERN Basic Backend with MongoDB Connection

A lightweight, beginner-friendly Node.js and Express backend with MongoDB integration using Mongoose.

## 🚀 Features

- Express.js REST API
- MongoDB connection using Mongoose
- Environment variables management via `dotenv`
- CORS enabled
- Basic CRUD operations for User model

---

## 🛠️ Tech Stack

- **Runtime:** [Node.js](https://nodejs.org/)
- **Framework:** [Express.js](https://expressjs.com/)
- **Database / ODM:** [MongoDB](https://www.mongodb.com/) / [Mongoose](https://mongoosejs.com/)
- **Dev Tool:** [Nodemon](https://nodemon.io/)

---

## 📋 Prerequisites

Make sure you have the following installed:
- [Node.js](https://nodejs.org/) (v16+ recommended)
- [MongoDB](https://www.mongodb.com/) (running locally or MongoDB Atlas connection string)

---

## ⚙️ Installation & Setup

1. **Clone the repository:**
   ```bash
   git clone https://github.com/riteshbhende/Mern_basic-with-db_connection.git
   cd Mern_basic-with-db_connection
   ```

2. **Install dependencies:**
   ```bash
   npm install
   ```

3. **Configure Environment Variables:**
   Create a `.env` file in the root directory (you can copy `.env.example`):
   ```env
   PORT=8080
   MONGO_URI=mongodb://127.0.0.1:27017/mern_beginner
   ```

4. **Run the server:**
   - **Development mode (with auto-reload):**
     ```bash
     npm run dev
     ```
   - **Production mode:**
     ```bash
     npm start
     ```

   The server will start on `http://localhost:8080`.

---

## 📡 API Endpoints

### Base URL: `http://localhost:8080`

| Method | Endpoint | Description |
| :--- | :--- | :--- |
| `GET` | `/` | Health check / Welcome message |
| `GET` | `/api/users` | Get all users |
| `GET` | `/api/users/:id` | Get single user by ID |
| `POST` | `/api/users` | Create a new user |
| `DELETE` | `/api/users/:id` | Delete a user by ID |

### Example Request Body for `POST /api/users`:
```json
{
  "name": "John Doe",
  "email": "john@example.com",
  "age": 25
}
```

---

## 📁 Project Structure

```
├── models/
│   └── User.js          # Mongoose User Schema
├── routes/
│   └── userRoutes.js    # User API routes
├── .env.example         # Example environment variables
├── .gitignore           # Git ignore file
├── package.json         # Project dependencies and scripts
├── README.md            # Project documentation
└── server.js            # Main server entry point
```

---

## 📄 License

This project is licensed under the [ISC License](LICENSE).
