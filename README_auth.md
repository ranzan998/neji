# NEJI Authentication System

A secure, full-stack web application for user registration and authentication with Node.js, Express, SQLite, and JWT tokens.

## Features

- **Secure Registration**: Email/password registration with strong password requirements
- **Secure Login**: Bcrypt password hashing with JWT token authentication
- **Protected Routes**: Dashboard accessible only to authenticated users
- **Session Management**: Automatic token validation and logout functionality
- **Real-time Validation**: Client-side form validation with visual feedback
- **Responsive Design**: Mobile-friendly interface matching NEJI branding
- **Security Best Practices**: Protection against common vulnerabilities

## Security Features

- **Password Hashing**: Bcrypt with 12 salt rounds
- **JWT Authentication**: Secure token-based authentication
- **Input Validation**: Server-side and client-side validation
- **SQL Injection Protection**: Parameterized queries
- **CORS Protection**: Configurable cross-origin resource sharing
- **Password Strength**: Enforced strong password requirements

## Prerequisites

- Node.js (v14 or higher)
- npm or yarn package manager

## Installation

1. **Clone or download the project files**

2. **Install dependencies:**
   ```bash
   npm install
   ```

3. **Set up environment variables:**
   ```bash
   cp .env.example .env
   ```
   
   Edit `.env` and update the JWT secret:
   ```bash
   # Generate a secure JWT secret
   node -e "console.log(require('crypto').randomBytes(64).toString('hex'))"
   ```

4. **Create the public directory structure:**
   ```
   project-root/
   ├── server.js
   ├── package.json
   ├── .env
   └── public/
       ├── index.html (your existing home page)
       ├── login_register.html

       
