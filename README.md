# ARIA — Teri AI Yaari 🌟

Your Hinglish AI friend, powered by Claude. Full animations, live unscripted responses.

---

## 🚀 Deploy in 5 minutes

### Option A — Render (Free, easiest)
1. Push this repo to GitHub
2. Go to [render.com](https://render.com) → New → Web Service
3. Connect your GitHub repo
4. Set:
   - **Build Command:** `npm install`
   - **Start Command:** `npm start`
5. Add environment variable:
   - `ANTHROPIC_API_KEY` = your key from [console.anthropic.com](https://console.anthropic.com)
6. Deploy → done ✅

### Option B — Railway
1. Push to GitHub
2. Go to [railway.app](https://railway.app) → New Project → Deploy from GitHub
3. Add variable: `ANTHROPIC_API_KEY` = your key
4. Done ✅

### Option C — Vercel (needs small tweak)
Vercel doesn't run Express well. Use Render or Railway instead.

---

## 💻 Run locally

```bash
git clone <your-repo>
cd aria-friend
npm install
cp .env.example .env
# Edit .env and add your ANTHROPIC_API_KEY
npm start
# Open http://localhost:3000
```

---

## 📁 Structure

```
aria-friend/
├── server.js          # Express backend — proxies Anthropic API
├── public/
│   └── index.html     # Full ARIA frontend
├── package.json
├── .env.example
└── .gitignore         # .env is gitignored — key stays safe
```

---

## 🔑 Get your API key

1. Go to [console.anthropic.com](https://console.anthropic.com)
2. API Keys → Create Key
3. Paste it as `ANTHROPIC_API_KEY` in your deploy platform's environment variables

**Never commit your `.env` file.** It's already in `.gitignore`.
