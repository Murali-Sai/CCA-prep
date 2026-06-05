# CCA Speedrun — 30-Day Claude Certified Architect Study Hub

A single-page, static study hub for the Anthropic **Claude Certified Architect — Foundations** exam.
Beginner-friendly concept primers, a day-by-day roadmap (study → build → drill), every free resource
linked, an interview-prep section, and built-in progress tracking (saved in your browser).

## What's inside
- `index.html` — the whole site (no build step, no dependencies)
- `resources/cca-exam-guide.pdf` — official exam guide
- `resources/architects-playbook.pdf` — the visual patterns playbook
- `vercel.json` — static-site config

## Deploy to Vercel (pick one)

**A. Drag & drop** — go to https://vercel.com/new, sign in, drag this folder onto the page, Deploy.

**B. GitHub**
```bash
git init && git add . && git commit -m "CCA study hub"
git branch -M main
git remote add origin https://github.com/<you>/cca-speedrun.git
git push -u origin main
# then import the repo at vercel.com/new (framework preset: Other)
```

**C. CLI**
```bash
npm i -g vercel
vercel        # preview
vercel --prod # production
```

## Run locally
Just open `index.html` in a browser, or:
```bash
python3 -m http.server 8000   # then visit http://localhost:8000
```

## Notes
- The Playbook PDF is ~14 MB (fine for Vercel). To shrink the deploy, delete `resources/`
  and keep the PDFs locally — the rest of the site is unaffected.
- Progress is stored in your browser's localStorage (per-device).
- Not affiliated with Anthropic. Confirm exam details on the official Skilljar page.
