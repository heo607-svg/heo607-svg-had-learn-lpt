# had.ai 🎓

> AI-powered study assistant — upload documents, get instant analysis, FAQs, and mock tests.

---

## 📁 Folder Structure

```
had-ai/
├── public/
│   └── index.html          → HTML shell
├── src/
│   ├── App.jsx             → Main React app
│   ├── api.js              → All backend API calls
│   ├── config.js           → Environment config
│   ├── index.js            → React entry point
│   └── index.css           → Global styles
├── server/
│   ├── server.js           → Express backend
│   └── package.json        → Backend dependencies
├── .env.example            → Copy this to .env
├── .gitignore
├── vercel.json             → Vercel deployment config
├── render.yaml             → Render deployment config
└── package.json            → Frontend dependencies
```

---

## 🚀 Run Locally

### 1. Clone and install
```bash
git clone https://github.com/YOUR_USERNAME/had-ai.git
cd had-ai
npm install
cd server && npm install && cd ..
```

### 2. Set up environment
```bash
cp .env.example .env
# Edit .env and add your Claude API key
```

### 3. Run frontend
```bash
npm start
# Opens at http://localhost:3000
```

### 4. Run backend (new terminal)
```bash
node server/server.js
# Runs at http://localhost:5000
```

---

## 🌐 Deploy

### Frontend → Vercel
1. Push to GitHub
2. Import repo on vercel.com
3. Add env variables
4. Deploy

### Backend → Render
1. Import repo on render.com
2. Set Root Directory to `server`
3. Add env variables
4. Deploy

---

## 🔑 Environment Variables

| Variable | Where | Description |
|----------|-------|-------------|
| `CLAUDE_KEY` | Backend (.env) | Claude API key |
| `REACT_APP_CLAUDE_KEY` | Frontend (.env) | Claude API key |
| `REACT_APP_BACKEND_URL` | Frontend (.env) | Backend URL |
| `FRONTEND_URL` | Backend (.env) | Frontend URL for CORS |

---

## 💳 Plans

| Plan | Price | Limit |
|------|-------|-------|
| Free | ₹0 | 9 uses, 15MB/file |
| Pro | ₹299/mo or ₹999/yr | Unlimited, 40MB/file |
| Ultra | ₹499/mo or ₹2999/yr | All features + Hybrid Tests |

---

## 🛠 Tech Stack

- **Frontend**: React 18
- **Backend**: Node.js + Express
- **AI**: Claude API (Anthropic)
- **File Parsing**: pdf-parse + mammoth
- **Deploy**: Vercel (frontend) + Render (backend)
