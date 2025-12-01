# Day-1-Backend-Revise
Node.js architecture, NPM basics, and professional backend setup using Express.

---

```md
# 📘 Backend Revision – Day 1

This repository contains **Day 1** of my backend revision streak.  
Today I revised: **Node.js architecture, NPM basics, and professional backend setup using Express.**

---

## 🚀 What I Revised Today

### ✅ Node.js Architecture
- Single-threaded event loop  
- Non-blocking I/O model  
- Asynchronous request handling  
- ES Modules  
- Middleware & Routing  
- Environment variables  

---

## 📦 NPM Basics
```

npm init -y
npm install express dotenv
npm install nodemon -D
npm run dev

```

**Key Files:**
- `package.json`  
- `package-lock.json`  
- `node_modules/`  

---

## 🗂️ Project Folder Structure


backend-revision-day1/
│── src/
│   ├── config/
│   │    └── db.js
│   ├── routes/
│   │    └── user.routes.js
│   ├── controllers/
│   │    └── user.controller.js
│   ├── app.js
│── .env
│── .gitignore
│── package.json
│── README.md



---

## 🧪 Starter Code

### `src/app.js`
```js
import express from "express";
import dotenv from "dotenv";

dotenv.config();
const app = express();

app.use(express.json());

app.get("/", (req, res) => {
  res.send("Backend Revision Day 1 Working 🚀");
});

const PORT = process.env.PORT || 5000;
app.listen(PORT, () => console.log(`Server running on port ${PORT}`));
````

### `.env`

```
PORT=5000
```

### `.gitignore`

```
node_modules/
.env
```

---

## ▶️ How to Run

```
npm install
npm run dev
```

Visit:
**[http://localhost:5000](http://localhost:5000)**

---

## 🔼 GitHub Push Steps

```
git init
git add .
git commit -m "Day 1 backend revision setup"
git branch -M main
git remote add origin <your_repo_url>
git push -u origin main
```

---

# 🟢 Day 1 Completed!

This is the start of my backend revision streak.

**Streak Progress**

* ✔️ Day 1 — Node + NPM + Setup
---

# ⭐ Notes for Future Me

* Stay consistent
* Upload every day
* Even small progress counts

```

🔥 Shorter (if interviewer wants concise answer):

“Node.js is single-threaded and uses an event loop to handle asynchronous operations, allowing it to process many requests at the same time without blocking.”

⭐ If they ask WHY this is useful:

“Because it avoids thread creation overhead, reduces memory usage, and makes Node.js extremely fast for I/O-heavy applications.”

🧠 If they ask HOW it works:

“The main thread runs the event loop. Long-running tasks like I/O are sent to worker threads in the background. When they finish, callbacks are queued and executed by the event loop.”

---

