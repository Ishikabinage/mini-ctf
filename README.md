# ⚡ PROJECT AURA — CTF Platform

<div align="center">

![Project AURA](https://img.shields.io/badge/PROJECT-AURA-00f5d4?style=for-the-badge&labelColor=050a0e&color=00f5d4)
![Python](https://img.shields.io/badge/Python-3.11-blue?style=for-the-badge&logo=python&logoColor=white&labelColor=050a0e)
![Flask](https://img.shields.io/badge/Flask-2.x-green?style=for-the-badge&logo=flask&logoColor=white&labelColor=050a0e)
![SQLite](https://img.shields.io/badge/SQLite-Database-orange?style=for-the-badge&logo=sqlite&logoColor=white&labelColor=050a0e)
![Status](https://img.shields.io/badge/Status-LIVE-00f5d4?style=for-the-badge&labelColor=050a0e)

**A two-player Capture The Flag platform built for a hackathon.**  
*Progressive challenge unlocks · Live scoreboard · Cyberpunk terminal UI*

[▶ Play Now](#) · [Report Bug](https://github.com/ShreyashNaik30/mini-ctf/issues) · [View Challenges](#challenges)

</div>

---

## 🖥️ Preview

> Cyberpunk terminal-themed interface with glitch animations, challenge popups, and a live scoreboard.

```
[ PROJECT AURA ] _
> Agent authenticated // SECURE CHANNEL ACTIVE
// MISSION_CONTROL::CHALLENGE_MATRIX
```

---

## 🚀 Features

- 🔐 **Secure Login** — Hashed passwords, session management via Flask-Login. Wrong credentials trigger a shake animation — no plain white error pages.
- 🧩 **9 Progressive Challenges** — Each correct flag submission unlocks the next level. Challenges span logic, encoding, pattern recognition, cryptography, and web inspection.
- ⚡ **Instant Flag Feedback** — AJAX-powered submission with animated popups. Correct = glitch effect + redirect. Wrong = shake + red flash.
- 🏆 **Live Scoreboard** — Real-time rankings with gold/silver rank badges and status tiers (ACTIVE → ADVANCED → ELITE).
- 🎨 **Cyberpunk UI** — Grid scanlines, Orbitron font, teal glow effects, card hover animations — built from scratch with pure CSS.

---

## 🧩 Challenges

| # | Title | Category | Points |
|---|-------|----------|--------|
| 1 | Boot Sequence Recovery | Logic / Math | 50 |
| 2 | Memory Parser | String Manipulation | 75 |
| 3 | Signal Decoder | Base64 Encoding | 100 |
| 4 | Logic Engine | Lateral Thinking | 100 |
| 5 | Pattern Analyzer | Pattern Recognition | 125 |
| 6 | Hidden Console | Web / Recon | 150 |
| 7 | Encryption Node | Caesar Cipher | 175 |
| 8 | System Patch | Code Debugging | 200 |
| 9 | Core Vault | Meta / OSINT | 300 |

> Total possible score: **1275 pts**

---

## 🛠️ Tech Stack

| Layer | Technology |
|-------|-----------|
| Backend | Python 3, Flask |
| Database | SQLite + Flask-SQLAlchemy |
| Auth | Flask-Login + Werkzeug password hashing |
| Frontend | Jinja2 templates, vanilla CSS, vanilla JS |
| Fonts | Orbitron, Share Tech Mono, Rajdhani |
| Deployment | Render (Gunicorn) |

---

## ⚙️ Local Setup

```bash
# 1. Clone the repo
git clone https://github.com/ShreyashNaik30/mini-ctf.git
cd mini-ctf

# 2. Create and activate virtual environment
python -m venv venv
venv\Scripts\activate        # Windows
# source venv/bin/activate   # Mac/Linux

# 3. Install dependencies
pip install -r requirements.txt

# 4. Run the app
python app.py

# 5. Initialize database (run once)
# Visit: http://127.0.0.1:5000/setup
```

---

## 🌐 Deployment (Render)

1. Push to GitHub
2. Connect repo on [render.com](https://render.com)
3. Set **Build Command:** `pip install -r requirements.txt`
4. Set **Start Command:** `gunicorn app:app`
5. Deploy → visit `/setup` once to initialize DB

---

## 👥 Players

| Agent | Username |
|-------|----------|
| 🧠 Ishika Binage | `Ishika` |
| ⚡ Shreyash Naik | `Shreyash` |

---

## 📁 Project Structure

```
mini-ctf/
├── app.py                  # Flask app, routes, models
├── requirements.txt        # Python dependencies
├── Procfile                # Render start command
├── templates/
│   ├── base.html           # Navbar, layout, scanline effects
│   ├── login.html          # Auth page with shake animation
│   ├── dashboard.html      # Challenge grid
│   ├── challenge.html      # Flag submission + popup
│   └── scoreboard.html     # Live leaderboard
└── static/
    └── style.css           # Full cyberpunk theme
```

---

## 📜 License

Built for a hackathon. Open for anyone to fork, remix, and play. ⚡

---

<div align="center">

Made with 🖤 by **Ishika Binage** & **Shreyash Naik**

*// AURA SYSTEM v1.0 // SECURE TERMINAL //*

</div>