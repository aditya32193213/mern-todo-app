<div align="center">

# ✅ TaskFlow

### *Your tasks. Your flow. Totally under control.*

[![Live Demo](https://img.shields.io/badge/🌐_Frontend-Live_Demo-6366f1?style=for-the-badge)](https://todo-frontend-swart-nine.vercel.app/)
[![Backend API](https://img.shields.io/badge/⚙️_Backend-API_Docs-10b981?style=for-the-badge)](https://todo-backend-t5gm.onrender.com/)
[![License: MIT](https://img.shields.io/badge/📄_License-MIT-f59e0b?style=for-the-badge)](LICENSE)
[![PRs Welcome](https://img.shields.io/badge/🤝_PRs-Welcome-ec4899?style=for-the-badge)](CONTRIBUTING.md)

<br/>

> 🚀 A **full-stack productivity powerhouse** — create, organize, and conquer your tasks with a sleek UI and a rock-solid REST API.

<br/>

---

## 🎬 Demo

[![TaskFlow Demo Video](https://img.shields.io/badge/▶️_Watch_Demo-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.loom.com/share/cf2456f629684cfeaec0441862e4416d)

> 📹 *Click above to watch a full walkthrough of TaskFlow in action!*

---

</div>

## 🌟 Features

- ✏️ **Create & Edit Tasks** — Add tasks instantly with titles, descriptions, and due dates
- ✅ **Mark Complete** — One-click task completion with satisfying visual feedback
- 🗑️ **Delete Tasks** — Clean up your list with smooth animations
- 🔍 **Filter & Search** — Find any task in seconds by status or keyword
- 📱 **Fully Responsive** — Pixel-perfect on desktop, tablet, and mobile
- 🌙 **Dark Mode Ready** — Easy on the eyes, day or night
- ⚡ **Blazing Fast** — Optimistic UI updates with real-time sync to the backend
- 🔐 **Secure REST API** — Robust backend with validation and error handling

---

## 🛠️ Tech Stack

### 🎨 Frontend
| Technology | Purpose |
|------------|---------|
| ⚛️ React | UI Framework |
| 🎨 Tailwind CSS | Styling |
| 🔄 Axios | HTTP Client |
| 🧭 React Router | Client-side Routing |
| 📦 Vite | Build Tool |

### ⚙️ Backend
| Technology | Purpose |
|------------|---------|
| 🟢 Node.js | Runtime |
| 🚂 Express.js | Web Framework |
| 🍃 MongoDB | Database |
| 🔗 Mongoose | ODM |
| 🛡️ CORS | Cross-Origin Support |

---

## 🚀 Live Links

| 🌐 Service | 🔗 URL |
|------------|--------|
| 🖥️ Frontend App | [Click here to open the app](https://todo-frontend-swart-nine.vercel.app/) |
| ⚙️ Backend API | [Click here to view the API](https://todo-backend-t5gm.onrender.com/) |
| 🎬 Demo Video | [Click here to watch the demo](https://www.loom.com/share/cf2456f629684cfeaec0441862e4416d) |

> ⚠️ *Replace the placeholders above with your actual deployed URLs.*

---

## 📁 Project Structure

```
taskflow/
├── 📂 client/                  # React Frontend
│   ├── 📂 src/
│   │   ├── 📂 components/      # Reusable UI components
│   │   │   ├── TaskCard.jsx
│   │   │   ├── TaskForm.jsx
│   │   │   └── FilterBar.jsx
│   │   ├── 📂 pages/           # Route-level pages
│   │   │   └── Home.jsx
│   │   ├── 📂 api/             # Axios API calls
│   │   │   └── tasks.js
│   │   ├── App.jsx
│   │   └── main.jsx
│   ├── index.html
│   └── package.json
│
├── 📂 server/                  # Express Backend
│   ├── 📂 models/
│   │   └── Task.js             # Mongoose schema
│   ├── 📂 routes/
│   │   └── tasks.js            # CRUD route handlers
│   ├── 📂 middleware/
│   │   └── errorHandler.js
│   ├── server.js               # Entry point
│   └── package.json
│
└── 📄 README.md
```

---

## ⚙️ Getting Started

### 📋 Prerequisites

Make sure you have the following installed:

- 🟢 **Node.js** v18+
- 🍃 **MongoDB** (local or Atlas cloud)
- 📦 **npm** or **yarn**

---

### 🔧 Installation

**1️⃣ Clone the repository**

```bash
git clone https://github.com/aditya32193213/mern-todo-app.git
cd taskflow
```

**2️⃣ Set up the Backend**

```bash
cd server
npm install
```

Create a `.env` file in the `server/` folder:

```env
PORT=5000
MONGO_URI=your_mongodb_connection_string_here
```

Start the server:

```bash
npm run dev
```

> 🟢 Backend running at `http://localhost:5000`

---

**3️⃣ Set up the Frontend**

```bash
cd ../client
npm install
```

Create a `.env` file in the `client/` folder:

```env
VITE_API_URL=http://localhost:5000/api
```

Start the dev server:

```bash
npm run dev
```

> 🎨 Frontend running at `http://localhost:5173`

---

## 📡 API Reference

Base URL: `YOUR_BACKEND_URL_HERE/api`

| 🔷 Method | 🔗 Endpoint | 📝 Description |
|----------|------------|---------------|
| `GET` | `/tasks` | 📋 Fetch all tasks |
| `POST` | `/tasks` | ➕ Create a new task |
| `PUT` | `/tasks/:id` | ✏️ Update a task |
| `PATCH` | `/tasks/:id/complete` | ✅ Toggle task completion |
| `DELETE` | `/tasks/:id` | 🗑️ Delete a task |

### 📦 Example Request — Create a Task

```json
POST /api/tasks
Content-Type: application/json

{
  "title": "Build something awesome 🚀",
  "description": "Work on the TaskFlow app",
  "dueDate": "2026-03-31"
}
```

### 📦 Example Response

```json
{
  "_id": "64abc123...",
  "title": "Build something awesome 🚀",
  "description": "Work on the TaskFlow app",
  "completed": false,
  "dueDate": "2026-03-31T00:00:00.000Z",
  "createdAt": "2026-03-21T10:00:00.000Z"
}
```

---

## 🧪 Running Tests

```bash
# Backend tests
cd server && npm test

# Frontend tests
cd client && npm test
```

---

## 🚢 Deployment

### 🎨 Frontend — [Vercel](https://vercel.com) / [Netlify](https://netlify.com)

```bash
cd client
npm run build
# Deploy the /dist folder
```

### ⚙️ Backend — [Render](https://render.com) / [Railway](https://railway.app)

- Set environment variables (`MONGO_URI`, `PORT`) in your hosting dashboard
- Connect your GitHub repo and deploy!

---

## 🤝 Contributing

Contributions are always welcome! 🎉

```bash
# 1. Fork the repo
# 2. Create your feature branch
git checkout -b feature/amazing-feature

# 3. Commit your changes
git commit -m "✨ Add some amazing feature"

# 4. Push to the branch
git push origin feature/amazing-feature

# 5. Open a Pull Request 🚀
```

---

## 🐛 Known Issues / Roadmap

- [ ] 🔐 User authentication & login
- [ ] 🏷️ Task categories & tags
- [ ] 📊 Productivity dashboard & stats
- [ ] 🔔 Due date reminders & notifications
- [ ] 🤝 Collaborative task sharing

---

## 📄 License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.

---

## 🙏 Acknowledgements

- 💙 [React](https://reactjs.org/) — For the magical UI library
- 🟢 [Express.js](https://expressjs.com/) — For the no-nonsense backend framework
- 🍃 [MongoDB](https://www.mongodb.com/) — For the flexible, scalable database
- 🎨 [Tailwind CSS](https://tailwindcss.com/) — For making CSS actually enjoyable

---

<div align="center">

Made with ❤️ and ☕ by **[Your Name](https://github.com/YOUR_USERNAME)**

⭐ *If you found this project helpful, please give it a star!* ⭐

[![GitHub stars](https://img.shields.io/github/stars/YOUR_USERNAME/taskflow?style=social)](https://github.com/YOUR_USERNAME/taskflow)
[![GitHub forks](https://img.shields.io/github/forks/YOUR_USERNAME/taskflow?style=social)](https://github.com/YOUR_USERNAME/taskflow/fork)

</div>
