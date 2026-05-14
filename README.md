<h1 align="center">💳 Banking Dashboard</h1>

<p align="center">
  A full-stack banking web app with facial recognition login, role-based dashboards, and real-time transaction management.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Stack-MERN-informational?logo=mongodb&logoColor=white" />
  <img src="https://img.shields.io/badge/Auth-Face%20Recognition%20%2B%20JWT-blueviolet" />
  <img src="https://img.shields.io/badge/UI-Tailwind%20CSS-38bdf8" />
  <img src="https://img.shields.io/badge/License-MIT-brightgreen" />
</p>

---

## ✨ Features

| Feature | Description |
|--------|-------------|
| 🎭 Face Recognition Login | Biometric authentication using `face-api.js` with JWT session handling |
| 🔐 Role-Based Access | Separate dashboards for Admin, Employee, and Customer roles |
| 💸 Transactions | Deposit, withdraw, and transfer with live balance updates |
| 🏦 Loan Management | Apply, review, and approve loan requests through a workflow |
| 🤖 AI Credit Score | GROQ-powered CIBIL score analysis and suggestions |
| 📱 Responsive Design | Fully responsive UI built with Tailwind CSS |

---

## 🛠️ Tech Stack

**Frontend** — React.js, Tailwind CSS, React Router, Axios  
**Backend** — Node.js, Express.js, Mongoose  
**Database** — MongoDB  
**Authentication** — face-api.js, JWT  
**AI** — GROQ API (OpenAI-compatible)

---

## ⚙️ Getting Started

### Prerequisites
- Node.js v18+
- MongoDB (local or Atlas)
- GROQ API key

### Installation

```bash
# 1. Clone the repo
git clone https://github.com/geyasrivagdevi/banking_dashboard.git
cd banking_dashboard

# 2. Backend setup
cd server
npm install

# 3. Create your environment file
# Create server/.env and add:
# MONGO_URI=your_mongodb_uri
# JWT_SECRET=your_jwt_secret
# GROQ_API_KEY=your_groq_key

npm start  # runs on http://localhost:5000

# 4. Frontend setup
cd ../client
npm install
npm run dev  # runs on http://localhost:5173
```

> 💡 On Windows, run `run.bat` from the root folder to start both servers at once.

---

## 📁 Project Structure

```
banking_dashboard/
├── client/          # React frontend
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   └── assets/
├── server/          # Express backend
│   ├── routes/
│   ├── controllers/
│   ├── models/
│   └── middlewares/
└── run.bat
```

---

## 🔑 Environment Variables

Create a `.env` file inside the `server/` folder:

```
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_secret_key
GROQ_API_KEY=your_groq_api_key
```

> ⚠️ Never commit your `.env` file. It's already in `.gitignore`.

---

## 🤝 Contributing

1. Fork the repo
2. Create a branch — `git checkout -b feature/your-feature`
3. Commit your changes — `git commit -m "Add your feature"`
4. Push — `git push origin feature/your-feature`
5. Open a Pull Request

---

## 📜 License

MIT © [Geyas Sri Vagdevi](https://github.com/geyasrivagdevi)

---

## 🙏 Acknowledgements

- [face-api.js](https://github.com/justadudewhohacks/face-api.js) for facial recognition
- [Tailwind CSS](https://tailwindcss.com/) for the UI
- [GROQ](https://groq.com/) for AI-powered credit analysis
