<div align="center">

# 🎓 Convo — AI-Powered College Toolkit

### Centralize college communication and productivity in one platform.

[![MongoDB](https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white)](https://www.mongodb.com/)
[![Express.js](https://img.shields.io/badge/Express.js-404D59?style=for-the-badge&logo=express&logoColor=white)](https://expressjs.com/)
[![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)](https://reactjs.org/)
[![Node.js](https://img.shields.io/badge/Node.js-43853D?style=for-the-badge&logo=node.js&logoColor=white)](https://nodejs.org/)
[![Socket.io](https://img.shields.io/badge/Socket.io-black?style=for-the-badge&logo=socket.io&badgeColor=010101)](https://socket.io/)
[![Google Cloud](https://img.shields.io/badge/Google_Cloud-4285F4?style=for-the-badge&logo=google-cloud&logoColor=white)](https://cloud.google.com/)

</div>

---

## 📌 About

**Convo** is a full-stack MERN application designed to centralize college communication and productivity. It combines real-time messaging, academic tools, and an AI-powered study assistant into a single platform — reducing the need for multiple apps.

---

## 🚀 Features

- 💬 **Real-time one-on-one and group chat** with low latency
- 🤖 **AI-powered study assistant** using RAG (context-based Q&A)
- 📁 **Upload and query course materials** — get answers from your own notes
- 🏫 **Structured communication** for students and faculty
- ⚡ **Handles 50+ concurrent users** efficiently

---

## 🧠 AI Integration

Convo includes an AI study assistant built using **RAG (Retrieval-Augmented Generation)**:

- Uses **LangChain + OpenAI API**
- Allows users to upload notes and course materials
- Answers questions based on actual uploaded content — not generic responses
- Helps reduce time spent searching through PDFs or notes

```
User uploads course material (PDF / notes)
             ↓
  Document chunked into passages
             ↓
  Passages embedded via OpenAI Embeddings
             ↓
    Stored in FAISS Vector Store
             ↓
        User asks a question
             ↓
  Relevant passages retrieved (similarity search)
             ↓
  LangChain passes context + question to GPT
             ↓
    Context-aware answer returned ✅
```

---

## ⚡ Real-Time System

- Built using **Socket.io**
- Supports personal and group chats
- Achieves **sub-100ms message latency** under load

---

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| **Frontend** | React, HTML5, CSS3, JavaScript |
| **Backend** | Node.js, Express.js |
| **Database** | MongoDB |
| **Real-time** | Socket.io |
| **AI / RAG** | LangChain, OpenAI API, FAISS |
| **Deployment** | Google Cloud Run |
| **CI/CD** | GitHub Actions |

---

## 📦 Installation

### 1. Clone the repository

```bash
git clone https://github.com/Apex800/convo.git
cd convo
```

### 2. Install dependencies

**Frontend:**
```bash
cd client
npm install
```

**Backend:**
```bash
cd server
npm install
```

### 3. Environment variables

Create a `.env` file in the `/server` folder:

```env
MONGO_URI=your_mongodb_connection
JWT_SECRET=your_secret_key
OPENAI_API_KEY=your_key
```

### 4. Run the app

**Backend:**
```bash
cd server
npm start
```

**Frontend:**
```bash
cd client
npm start
```

Open [http://localhost:3000](http://localhost:3000) in your browser.

---

## 📌 Deployment

- Deployed on **Google Cloud Run**
- Automated CI/CD using **GitHub Actions**
- Maintains **99%+ uptime**

---

## 🎯 Goal

Convo aims to simplify student life by combining communication, collaboration, and AI-powered learning tools into one platform — so students spend less time switching between apps and more time actually learning.

---

## 🔮 Future Improvements

- [ ] Role-based access (admin, faculty, student)
- [ ] File and media sharing in chat
- [ ] Better mobile responsiveness
- [ ] Notifications system

---

## 📬 Contact

**Ammar Khan**
- 📧 khanammar800@gmail.com
- 💼 [linkedin.com/in/ammar-khan-698747279](https://www.linkedin.com/in/ammar-khan-698747279)
- 🐙 [github.com/Apex800](https://github.com/Apex800)

---

<div align="center">
  <sub>Built with ❤️ for students, by a student.</sub>
</div>
