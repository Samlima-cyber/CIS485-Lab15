# Lab 15 – Using Cookies and Sessions in Node.js (CIS 485)

## 📚 Overview

This project demonstrates how to manage **cookies** and **sessions** in a Node.js Express app. The lab shows how to:

- Set, retrieve, and delete cookies
- Create and destroy user sessions
- Secure session and cookie data with middleware

## 🏗️ Technologies Used

- Node.js
- Express
- cookie-parser
- express-session

## 🚀 How to Run

1. Install dependencies:
   ```bash
   npm install
Start the server:

bash
Copy
Edit
node app.js
Open your browser and test the following routes:

Route	Description
/	Welcome page
/set-cookie	Sets a username cookie
/get-cookie	Retrieves cookie value
/delete-cookie	Deletes the cookie
/login	Starts a session
/profile	Displays session username
/logout	Destroys the session

🔐 Security Notes
The app uses httpOnly cookies to prevent client-side JS access.

In production, sessions should use secure: true with HTTPS and a session store (e.g., Redis).

📘 Reflection
1. What is the difference between cookies and sessions?
Cookies are stored in the browser, sessions are stored on the server. Cookies are sent with each request, while sessions keep sensitive data secure on the backend.

2. How can you make cookies and sessions more secure?
Use secure: true for HTTPS

Use httpOnly to block JS access

Store sessions in a DB like Redis instead of memory

3. When would you use a session vs a cookie?
Use sessions for login/authentication

Use cookies for lightweight, non-sensitive client preferences

👨‍💻 Author
Sam Lima
CIS 485 – Spring 2025
