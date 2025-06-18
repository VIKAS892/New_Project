# 🔐 Firebase Auth Frontend with Dashboard & Tools

A React-based frontend project using **Firebase Authentication**. Includes:
- Secure login/signup (Email/Password)
- Dashboard showing user info
- Profile section
- Tools listing page
- Protected routes

---

## 🌐 Live Demo

👉 [https://frontend-786.web.app](https://frontend-786.web.app)

---

## 🚀 Features

- ✅ Firebase Email/Password Login & Signup
- 🔐 Protected Routes using Context API
- 👤 Profile View & Update Section
- 🧰 Tools List Page (placeholder or real tools)
- 📤 Logout functionality

---

## 🧠 Tech Stack

- **React JS**
- **Firebase Auth**
- **React Router DOM**
- **React Context API**
- **Tailwind CSS** *(or plain CSS Modules)*

---

## 📁 Folder Structure

frontend-firebase-auth/
├── public/
│ └── index.html
├── src/
│ ├── components/
│ │ ├── Login.js
│ │ ├── Signup.js
│ │ ├── Dashboard.js
│ │ ├── Profile.js
│ │ └── Tools.js
│ ├── context/
│ │ └── AuthContext.js
│ ├── firebase.js
│ ├── App.js
│ └── index.js
├── firebase.json
├── .gitignore
├── package.json
└── README.md


---

## 🔧 Firebase Setup

1. Go to [Firebase Console](https://console.firebase.google.com)
2. Create a project
3. Enable **Authentication → Email/Password**
4. Copy the config and paste in `src/firebase.js`:

```js
import { initializeApp } from "firebase/app";
import { getAuth } from "firebase/auth";

const firebaseConfig = {
  apiKey: "YOUR_API_KEY",
  authDomain: "your-app.firebaseapp.com",
  projectId: "your-project-id",
  storageBucket: "your-app.appspot.com",
  messagingSenderId: "SENDER_ID",
  appId: "APP_ID"
};

const app = initializeApp(firebaseConfig);
export const auth = getAuth(app);


Build & Deploy to Firebase Hosting

npm run build
firebase deploy

🔮 Future Enhancements
Add Google OAuth login

Firebase Storage for profile images

Real-time chat integration

Connect to live backend APIs

Dark/light theme toggle

