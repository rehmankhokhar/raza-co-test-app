# 📄 ReactJS Frontend — Full-Stack Web Application

This is the **frontend ReactJS application** for the full-stack project demonstrating:

- Login authentication with JWT  
- Role-based dashboard (Admin/User)  
- Responsive UI with Header and Footer  
- Integration with .NET 10 Web API backend  
- Handles login, token storage, and role-based content rendering  

---

## 🔹 Features

- **Login Page**:
  - Validates username and password fields  
  - Displays error messages for incorrect credentials  
- **Dashboard Page**:
  - Displays welcome message: "Welcome, [username]!"  
  - Role-based content:
    - Admin → "Admin Dashboard"  
    - User → "User Dashboard"  
- **JWT Handling**:
  - Stores JWT token in `localStorage`  
  - Sends token in `Authorization` header for API requests  
  - Redirects to login page if not authenticated  
- **Responsive UI**:
  - Works on desktop and mobile devices  
  - Includes Header and Footer components  

---

## 🔹 Prerequisites

- [Node.js](https://nodejs.org/) v18+  
- npm  

---

## 🔹 Setup & Run

1. Clone the repository:

```bash
git clone <repo-url>
cd frontend
npm install
npm start
http://localhost:3000
| Role  | Username | Password |
| ----- | -------- | -------- |
| Admin | admin    | 123456   |
| User  | user     | 123456  |

/src
  /components   → Header, Footer, shared components
  /pages        → Login, Dashboard pages
  /services     → API services (axios/fetch)
  /context      → JWT and authentication context (optional)
  App.js        → Main app with routing

