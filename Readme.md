# 🚀 MegaBackend - Industrial Grade Node.js Backend

[![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)](https://nodejs.org/)
[![Express.js](https://img.shields.io/badge/Express.js-000000?style=for-the-badge&logo=express&logoColor=white)](https://expressjs.com/)
[![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white)](https://www.mongodb.com/)
[![Cloudinary](https://img.shields.io/badge/Cloudinary-3448C5?style=for-the-badge&logo=cloudinary&logoColor=white)](https://cloudinary.com/)
[![JWT](https://img.shields.io/badge/JWT-black?style=for-the-badge&logo=JSON%20web%20tokens)](https://jwt.io/)

A robust, scalable, and highly secure Node.js backend architecture built with **Express.js**, **MongoDB**, and **Cloudinary**. This project follows industry-best practices for building enterprise-level applications, featuring a production-ready folder structure, advanced database modeling, and professional security implementation.

## 🌟 Key Features

- **🔐 Professional Authentication**: Robust JWT-based authentication system with Access and Refresh tokens (HttpOnly cookies).
- **🛡️ Secure Pw Hashing**: Industry-standard password hashing using `bcrypt`.
- **☁️ Integrated Media Management**: Seamless integration with **Cloudinary** for high-efficiency image and video storage.
- **🏗️ Industrial Folder Structure**: Clean separation of concerns (Controllers, Models, Routes, Middlewares, Utils).
- **📉 Advanced DB Operations**: Complex aggregation pipelines for fetching watch history, channel profiles, and subscriber counts.
- **🚀 Scalable Architecture**: Designed to handle high-traffic API requests with optimized performance.
- **📁 File Handling**: Professional file upload handling using `Multer`.
- **💥 Centralized Error Handling**: Standardized `ApiError` and `ApiResponse` classes for consistent API communication.

---

## 🛠️ Tech Stack

- **Core**: JavaScript (ES6+), Node.js
- **Framework**: Express.js
- **Database**: MongoDB (Mongoose ORM)
- **Security**: JWT, Bcrypt, CORS, Cookie-parser
- **File Storage**: Cloudinary, Multer
- **Validation**: Mongoose Schemas, Custom Logic

---

## 📂 Project Structure

```text
src/
├── controllers/    # Business logic for endpoints
├── db/             # Database connection configuration
├── middlewares/    # Authentication & upload middlewares
├── models/         # Mongoose schemas & data modeling
├── routes/         # API endpoint declarations
├── utils/          # Standardized error/response helpers
├── app.js          # Express app configuration
└── index.js        # Server entry point
```

---

## 🚀 Getting Started

### Prerequisites

- Node.js installed
- MongoDB URI (Atlas or Local)
- Cloudinary Credentials

### Installation

1.  **Clone the repository**
    ```bash
    git clone https://github.com/Varni1512/backend-project.git
    cd backend-project
    ```

2.  **Install dependencies**
    ```bash
    npm install
    ```

3.  **Setup Environment Variables**
    Create a `.env` file in the root directory and add:
    ```env
    PORT=8000
    MONGODB_URI=your_mongodb_uri
    CORS_ORIGIN=*
    ACCESS_TOKEN_SECRET=your_secret
    ACCESS_TOKEN_EXPIRY=1d
    REFRESH_TOKEN_SECRET=your_secret
    REFRESH_TOKEN_EXPIRY=10d
    CLOUDINARY_CLOUD_NAME=your_name
    CLOUDINARY_API_KEY=your_key
    CLOUDINARY_API_SECRET=your_secret
    ```

4.  **Run the application**
    ```bash
    npm run dev
    ```

---

## 🛤️ Core API Endpoints

### 👤 User Endpoints
- `POST /api/v1/users/register` - Register a new user (with Avatar/Cover image)
- `POST /api/v1/users/login` - User Login
- `POST /api/v1/users/logout` - User Logout (Secured)
- `POST /api/v1/users/refresh-token` - Renew Access Token
- `GET /api/v1/users/current-user` - Get Profile details
- `PATCH /api/v1/users/update-account` - Update name/email
- `PATCH /api/v1/users/avatar` - Update Avatar

---

## 🤝 Contribution

Contributions, issues, and feature requests are welcome! Feel free to check the [issues page](https://github.com/Varni1512/backend-project/issues).

## 📝 License

Distributed under the MIT License. See `LICENSE` for more information.

---
Created with ❤️ by [Varnikumar Patel](https://github.com/Varni1512)