# MERN-Multi-Level-Category-Management-API

MERN Multi-Level Category Management API

Overview

This is a Multi-Level Category Management API built using the MERN stack (MongoDB, Express.js, React, Node.js). The API supports JWT authentication, nested category management, and follows industry best practices.

Features

Authentication (JWT-based)

User registration & login.

Protect API routes using JWT middleware.

Category Management

Create a category (with optional parent).

Fetch all categories in a tree structure.

Update category name or status.

Delete a category and reassign its subcategories.

Bulk update subcategories when parent status changes.

Performance Optimizations

MongoDB Indexing for efficient queries.

Optimized tree structure retrieval.

Bulk updates handled efficiently.

Tech Stack

Backend: Node.js, Express.js, MongoDB (Mongoose ORM), JWT

Frontend: React (for category management UI)

Tools: Postman (API testing), Git (Version Control)

Installation & Setup

1️⃣ Clone the Repository
git clone https://github.com/yourusername/mern-category-management.git
 cd mern-category-management
 
2️⃣ Backend Setup
cd backend
 npm install

Create a .env file in backend/:
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_secret_key
PORT=5000
Run the server:

3️⃣ Frontend Setup
cd frontend
 npm install
 npm start

 API Routes

Auth Routes

POST /api/auth/register → Register user

POST /api/auth/login → Login and get JWT

Category Routes

POST /api/category → Create category

GET /api/category → Fetch categories as tree

PUT /api/category/:id → Update category

DELETE /api/category/:id → Delete category & reassign subcategories

Contribution

Fork the repository.

Create a new branch (feature-xyz).

Commit changes with meaningful messages.

Open a Pull Request.
