# PaintTrack Pro — Construction Track

A single-page construction paint-tracking dashboard built with pure HTML, CSS, and JavaScript. No build step required.

## Features
- Multi-theme UI (Ocean, Dark, Sunset, Forest, Light)
- Building / Floor / Location / Work-Type analytics
- Contractor assignment & row-splitting
- LocalStorage persistence — works fully offline in the browser

## Project Structure
```
construction_track_pro/
├── index.html                  # Main application (entry point)
├── painttrack.html             # Alternate / legacy copy
├── paint_tower_management_app.html
├── vercel.json                 # Vercel deployment config
└── README.md
```

## Local Development
Just open `index.html` in your browser — no server needed.

Optionally serve with any static server:
```bash
npx serve .
```

## Deploy to Vercel

### Option A — Vercel CLI
```bash
npm i -g vercel
vercel          # follow the prompts; Framework = Other / Static
```

### Option B — Vercel Dashboard (recommended)
1. Push this repo to GitHub / GitLab / Bitbucket.
2. Go to [vercel.com/new](https://vercel.com/new) and import the repo.
3. On the "Configure Project" screen:
   - **Framework Preset** → `Other`
   - **Root Directory** → `construction_track_pro`
   - **Build Command** → *(leave empty)*
   - **Output Directory** → `.`
4. Click **Deploy** — done.

> `vercel.json` in this folder handles routing and security headers automatically.