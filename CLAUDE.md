# Alfonso's App Store

Personal app store and AI agent launcher. Vibe coded with AI, deployed on Vercel.

## Project structure

```
app-store/           ← this repo, deployed at Vercel
├── index.html       ← the main store page
└── apps/
    ├── dj-set-tracker/index.html
    ├── recipes/index.html
    └── tastes/index.html

../tracklist-api/    ← API for DJ Song Tracker (Vercel serverless)
../lead-intel-api/   ← API for Lead Intelligence agent (Vercel serverless)
../tastes/           ← Tastes app (Next.js, separate Vercel project)
```

## Apps

| App | Accent color | Description |
|-----|-------------|-------------|
| Song Tracker | Purple `#8b5cf6` | Paste YouTube DJ set or live concert → get songs |
| Tastes | Orange `#f97316` | Personal restaurant map |
| Ricettario | Green `#22c55e` | Personal recipe collection |

## AI Agents (all on Telegram)

| Agent | Personality | Bot | Does |
|-------|------------|-----|------|
| Optima Tracker | Donna | @optima_tracker_bot | Daily 8am pipeline summary |
| Lead Intelligence | James | @optima_lead_intel_bot | Researches inmobiliarias, generates outreach |
| DJ Song Tracker | Jimmy | @dj_set_tracker_bot | YouTube link → tracklist |

## Design system

- Background: `#0a0a0a`, surface: `#141414`
- Accent: purple `#8b5cf6`
- Font: Inter
- Mobile-first, PWA-ready
- Footer quote: Naval — "who has the clearest vision and the highest taste"

## Deploy

```bash
# The app-store folder is its own git repo
git add . && git commit -m "..." && git push
# Vercel auto-deploys on push
```
