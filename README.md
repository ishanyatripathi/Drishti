# Drishti Video Analytics Platform — Static Deployment

This repository contains the standalone, evaluation-ready static frontend for the **Drishti Intelligent Border Video Analytics Platform**.

## Contents
- `index.html` — Full responsive dashboard with GOI Identity header, live badges, tactical alert banner, interactive incident drawer with evidence snapshots, enlarged camera feed modal, and dynamic CSV export.
- `assets/` — Includes:
  - `Cam1.mp4` (Virtual Fence Restricted Zone Breach)
  - `Cam2.mp4` (Multi-Class Vehicle Detection & Tracking)
  - `Cam3.mp4` (Perimeter Human Detection)
  - `Cam4.mp4` (Automatic Number Plate Recognition - ANPR & HUD)
  - `Cam5.mp4` (Suspicious Nighttime Stairwell Activity)
  - `Cam6.mp4` (Facial Verification & Watchlist Matching)
  - Brand assets (`product_logo.png`, `favion.png`, `team_logo.png`)

---

## Local Testing
To preview the static frontend locally:
```bash
# Using Python
python -m http.server 8080

# Or using Node
npx serve .
```
Then open `http://localhost:8080` in your browser.

---

## Deploy to Vercel / Netlify / GitHub Pages

### Option A: Create a New GitHub Repository & Deploy to Vercel (Recommended)
1. Initialize a new git repository inside this folder:
   ```bash
   git init
   git add .
   git commit -m "Initial commit: Drishti static showcase"
   ```
2. Create a new repository on your GitHub account (e.g. `drishti-showcase`).
3. Link and push to your new repository:
   ```bash
   git remote add origin https://github.com/<your-username>/drishti-showcase.git
   git branch -M main
   git push -u origin main
   ```
4. Log into [vercel.com](https://vercel.com):
   - Click **Add New Project** -> **Import Git Repository**.
   - Select `drishti-showcase`.
   - Framework Preset: **Other** (Pure HTML / Static).
   - Click **Deploy**. Done in ~15 seconds!

### Option B: Deploy with Vercel CLI (1-Click without Git)
If you have Vercel CLI installed:
```bash
npx vercel deploy --prod
```

### Option C: Drag & Drop to Netlify
1. Go to [app.netlify.com/drop](https://app.netlify.com/drop).
2. Drag and drop the `drishti_frontend` folder.
3. Your site is live immediately with a free HTTPS URL.
