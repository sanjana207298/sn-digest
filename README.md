# SN·digest 🔭

A daily supernova paper reader that pulls the latest arXiv submissions and explains them in plain English using AI.

Built for researchers (especially newcomers) who want to stay on top of the supernova literature without drowning in jargon.

---

## What it does

- **Fetches** the latest supernova papers from arXiv every time you open it
- **Filters** by a curated keyword list (supernova, core-collapse, Ic-BL, kilonova, SLSN, GRB-SN, SN designations like SN 2023ixf, and more)
- **Tracks** which papers you've already seen — new ones are highlighted, old ones dimmed
- **Explains** each paper in plain English using Claude (Anthropic) or Gemini Flash (Google)
- **Exports** any paper + its AI analysis as a Markdown file, ready to paste into Obsidian, Notion, or any notes app

No installation. No backend. Just open the link.

---

## Live app

👉 **[yourusername.github.io/sn-digest](https://yourusername.github.io/sn-digest)**

*(replace with your actual GitHub Pages URL after setup)*

---

## Setup (5 minutes)

### 1. Fork or clone this repo

```bash
git clone https://github.com/yourusername/sn-digest.git
```

Or just download `index.html` — that's the entire app.

### 2. Enable GitHub Pages

1. Go to your repo on GitHub
2. **Settings** → **Pages**
3. Under *Source*, select **Deploy from a branch**
4. Choose **main** branch, **/ (root)** folder
5. Click **Save**

GitHub will give you a URL like `https://yourusername.github.io/sn-digest` within a minute.

### 3. Get a free AI key (optional but recommended)

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

### 4. Enter your key in the app

Open the app → click **Settings** → choose your backend → paste your key → it saves automatically in your browser. You never need to enter it again.

**Your key is stored only in your browser's local storage. It is never sent to GitHub or any server — only directly to the API you chose.**

---

## Using inside Claude.ai (free, no key needed)

If you have a Claude.ai subscription:

1. Download `index.html` from this repo
2. Open Claude.ai → start a new chat
3. Attach the file and say: *"Run this as an artifact"*
4. In Settings inside the app, select **Claude** — no key needed

This is the easiest way to get Claude-quality analysis for free.

---

## Sharing with your group

Just share the GitHub Pages URL. Each person:
- Can browse papers immediately with no setup
- Gets their own seen/unseen tracking (stored in their own browser)
- Can add their own free Gemini key for AI analysis

No shared accounts, no shared costs, no server to maintain.

---

## Keywords used for filtering

Papers are kept if their title or abstract matches any of:

`supernova` · `supernovae` · `sn ia/ib/ic/iin/iip/iib` · `type ia/ib/ic` · `core-collapse` · `ccsn` · `ic-bl` · `grb-sn` · `gamma-ray burst supernova` · `kilonova` · `slsn` · `superluminous` · `thermonuclear supernova` · `csm interaction` · `nebular phase` · `SN 20xx / AT 20xx` (individual designations)

The app also matches the bare word `SN` in titles and detects individual supernova designations like `SN 2023ixf` or `AT2024abc`.

---

## Tips

- **For deeper analysis**: Use the app for a quick overview, then paste interesting abstracts into Claude.ai chat for a more detailed conversation.
- **Export format**: The `.md` export works directly with Obsidian — just paste or drop the file into your vault.
- **arXiv timing**: arXiv batches submissions. Papers posted Friday–Sunday all appear Monday morning. If it looks quiet, check again Monday.

---

## Technical notes

- Single `index.html` file — no build step, no dependencies, no server
- arXiv API is free and requires no authentication
- API keys are stored in `localStorage` — browser only, never transmitted to GitHub
- Seen paper tracking uses `localStorage` — persists across browser sessions

---

## Contributing

PRs welcome. Ideas:
- Additional keyword suggestions
- Filter by subcategory (e.g. only Ic-BL, only thermonuclear)
- Save notes alongside papers
- Export to BibTeX

---

*Made for the supernova community. Not affiliated with arXiv, Anthropic, or Google.*
