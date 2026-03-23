# 🤖 DevOps AI Agent

> A free, self-hosted AI assistant for Docker, GitHub Actions, and deployments — powered by **Google Gemini**.

**Live demo:** `https://YOUR-USERNAME.github.io/devops-agent`

---

## ✨ Features

- 🐳 **Docker** — Dockerfiles, docker-compose, multi-stage builds, security hardening
- 🐙 **GitHub Actions** — CI/CD pipelines, branch protection, releases, PR automation
- 🚀 **Deployments** — Zero-downtime scripts, nginx, SSL, VPS setup, Kubernetes YAMLs
- 💬 Full conversation memory per session
- 📋 One-click copy for all code blocks
- 🆓 100% free — powered by Gemini Flash free tier (1M tokens/day)
- 🔒 API key stored only in your browser's localStorage — never in code

---

## 🚀 Deploy to GitHub Pages in 5 minutes

### Step 1 — Fork or clone this repo

```bash
git clone https://github.com/YOUR-USERNAME/devops-agent.git
cd devops-agent
```

### Step 2 — Enable GitHub Pages

1. Go to your repo on GitHub
2. Click **Settings** → **Pages** (left sidebar)
3. Under **Source**, select **GitHub Actions**
4. Click **Save**

### Step 3 — Push to main

```bash
git add .
git commit -m "deploy devops agent"
git push origin main
```

The GitHub Actions workflow (`.github/workflows/deploy.yml`) will automatically build and deploy your site.

### Step 4 — Access your site

After the workflow completes (~30 seconds), your agent is live at:

```
https://YOUR-USERNAME.github.io/devops-agent
```

---

## 🔑 Get a Free Gemini API Key

1. Go to [aistudio.google.com/app/apikey](https://aistudio.google.com/app/apikey)
2. Sign in with your Google account
3. Click **Create API Key**
4. Copy the key

> **Free tier:** 1,000,000 tokens/day · 15 requests/min · No credit card needed

---

## ⚙️ Configuration

When you open the app, click **⚙ Configure** in the top-right corner and enter:

| Field | Description |
|---|---|
| **Gemini API Key** | Your `AIzaSy...` key from Google AI Studio |
| **Model** | `gemini-2.0-flash` (recommended), or `gemini-1.5-flash` / `gemini-1.5-pro` |
| **Stack Context** | Optional: describe your stack (e.g. "Node.js, PostgreSQL, Ubuntu VPS") |

Your key is stored in **browser localStorage only** — it never leaves your device or gets committed to the repo.

---

## 🔒 Security — Key Safety

| ✅ Safe | ❌ Never do this |
|---|---|
| Type key in the Configure UI | Paste key into `index.html` |
| Key stored in localStorage | Commit key to git |
| Only sent to Google's API | Push key to GitHub |

---

## 📁 Repo Structure

```
devops-agent/
├── index.html                    # The entire app (single file)
├── .github/
│   └── workflows/
│       └── deploy.yml            # Auto-deploy to GitHub Pages on push
└── README.md
```

---

## 🛠 Local Development

No build step needed — just open the file directly:

```bash
open index.html
# or
python3 -m http.server 8080
# then visit http://localhost:8080
```

---

## 📝 License

MIT — free to use, modify, and self-host.
