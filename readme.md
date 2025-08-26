# 🚀 ProjManage Backend

## 📌 Overview
ProjectCamp API is a **RESTful backend service** built with **Node.js, Express, and MongoDB**.  
It powers a collaborative project management system with secure **authentication, role-based authorization, and project lifecycle management**.  

Currently, **Phase 1 (Authentication & Authorization)** has been implemented.  
Future phases will include **Project, Task, Subtask, and Notes management**.  

---

## ✨ Features Implemented 
- ✅ User Registration with Email Verification  
- ✅ Secure Login with JWT Authentication  
- ✅ Role-Based Access Control (Admin, Project Admin, Member)  
- ✅ Password Management (Change, Forgot, Reset)  
- ✅ Token Refresh Mechanism  
- ✅ Logout with Token Invalidation  
- ✅ Resend Verification Email  
- ✅ Current User Info Endpoint  

---
### 1️⃣ Clone the Repository
```bash

git clone <(https://github.com/Suyash-Sahu/ProjManage-Backend.git)>
cd projectmanagement
```


## 📦 Install Dependencies

Run the following command to install all required packages:

```bash
npm install
```

## 📂 Project Structure
projectmanagement
├── node_modules
├── public
│   └── images
└── src
    ├── controllers
    ├── database
    ├── middlewares
    ├── models
    ├── routes
    ├── utils
    └── validators

## 🔧 Setup Environment Variables

Create a `.env` file in the project root and add the following variables:

```env
 🌐 Database
MONGO_URI=your_mongodb_connection_string

 ⚙️ Server
PORT=8000
CORS_ORIGIN=*

 🔑 JWT Authentication
ACCESS_TOKEN_SECRET=your_access_token_secret
ACCESS_TOKEN_EXPIRY=15m   # e.g., 15m, 1h, 7d
REFRESH_TOKEN_SECRET=your_refresh_token_secret
REFRESH_TOKEN_EXPIRY=7d   # e.g., 7d, 30d

 📧 Mailtrap (for testing emails)
MAILTRAP_SMTP_HOST=smtp.mailtrap.io
MAILTRAP_SMTP_PORT=2525
MAILTRAP_SMTP_USER=your_mailtrap_username
MAILTRAP_SMTP_PASS=your_mailtrap_password

FORGOT_PASSWORD_REDIRECT_URL=http://localhost:3000/forgot-password
```

## ⚡ Run the Server

For development (with auto-reload using nodemon):
```bash
npm run dev
```
For Production:
```bash
npm start
```


## 🛠️ Tech Stack
- **Backend:** Node.js, Express.js  
- **Database:** MongoDB (Mongoose ODM)  
- **Authentication:** JWT, Refresh Tokens  
- **Email Service:** Nodemailer (for verification & reset links)  
- **Validation:** Express Validator  
- **File Upload (Planned):** Multer  
- **Testing:** Postman  

---




