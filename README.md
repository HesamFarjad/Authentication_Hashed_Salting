# Authentication_Hashed_Salting
 Implements authentication with password security through hashing and salting using the "bcrypt" algorithm.


## 📌 Description

This is a basic user authentication system built with **Node.js**, **Express**, and **PostgreSQL**, with a strong focus on password security.  
Instead of storing plain text passwords, this version hashes and salts passwords before saving them to the database. The `bcrypt` library is used for secure password handling during both registration and login.

## ✅ Features

- User registration with hashed and salted passwords
- User login with bcrypt-based password comparison
- Secure storage of credentials in PostgreSQL
- Clean and minimal UI rendered with EJS
- Error handling for duplicate registrations and failed logins

## 🛠️ Technologies Used

- Node.js
- Express.js
- PostgreSQL
- Bcrypt
- EJS
- body-parser


![Screenshot 2025-06-14 at 12 37 04](https://github.com/user-attachments/assets/51eb1ea4-8b02-40ee-b62a-73d99134e533)


## 🧪 How It Works

### Registration Flow

1. User submits an email and password.
2. Password is **hashed and salted** using `bcrypt.hash()`.
3. Hashed password and email are stored in the `users` table.

### Login Flow

1. User submits login credentials.
2. The entered password is compared to the stored hashed password using `bcrypt.compare()`.
3. If it matches, user is authenticated.

## 🧱 Database Schema

<img width="1436" alt="Screenshot 2025-06-15 at 16 43 54" src="https://github.com/user-attachments/assets/9f7bd1db-2061-4e25-8025-69aa77b8d68e" />

