# SN·digest 

A daily supernova paper reader that pulls the latest arXiv submissions and explains them in plain English using AI.

Built for researchers (especially newcomers) who want to stay on top of the supernova literature.

---

## What it does

- **Fetches** the latest supernova papers from arXiv every time you open it
- **Filters** by a curated keyword list (supernova, core-collapse, Ic-BL, SLSN, GRB-SN, and more)
- **Tracks** which papers you've already seen — new ones are highlighted, old ones dimmed
- **Explains** each paper in plain English using Claude (Anthropic) or Gemini Flash (Google)
- **Exports** any paper + its AI analysis as a Markdown file, ready to paste into Obsidian, Notion, or any notes app

No installation. No backend. Just open the link.

---

## Live app

**[sanjana207298.github.io/sn-digest](https://sanjana207298.github.io/sn-digest)**

---

## Setup

### 1. Fork or clone this repo

```bash
git clone https://github.com/yourusername/sn-digest.git
```

Or just download `index.html` — that's the entire app.

### 2. Get a free AI key 

The app works without any key — you can browse abstracts and arXiv links for free. For AI-generated explanations, you need one of:

**Option A — Gemini Flash (Google, free)**
- Go to [aistudio.google.com](https://aistudio.google.com)
- Click *Get API key* → Create
- Free tier: 1,500 analyses per day

**Option B — Claude (Anthropic, paid)**
- Go to [console.anthropic.com](https://console.anthropic.com)
- Create an account and add billing
- ~$0.003 per paper analysis (very cheap)
- Better quality explanations

### 3. Enter your key in the app

Open the app → click **Settings** → choose your backend → paste your key → it saves automatically in your browser. 

**Your key is stored only in your browser's local storage. It is never sent to GitHub or any server — only directly to the API you chose.**

---

## Using inside Claude.ai (free, no key needed)

If you have a Claude.ai subscription:

1. Download `index.html` from this repo
2. Open Claude.ai → start a new chat
3. Attach the file and say: *"Run this as an artifact"*
4. In Settings inside the app, select **Claude** — no key needed
