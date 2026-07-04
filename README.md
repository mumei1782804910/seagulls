# 🏖️ Seagull Hunt

A cute, mobile-friendly beach game. Five seagulls are hiding on a sandy grid —
you have 20 tile flips to find them all! The seagulls walk around between your
flips, leaving hidden footprints behind. Footprints only show up when you flip
the tile they're on, so use them to track the birds down.

## How to play

- 👆 Flip a sand tile to check for a seagull. Every flip counts!
- 👣 Footprints mean a seagull walked off that tile — it's somewhere nearby.
- 🏖️ Plain sand means nothing has been there (so far...).
- 🎯 A found seagull stays put and stops walking.
- 🔍 Find all 5 seagulls before your 20 flips run out, or they escape.

## Play locally

Just open `index.html` in any browser, or serve it:

```bash
python3 -m http.server 8000
# then visit http://localhost:8000 on your phone (same Wi-Fi, use your computer's IP)
```

## Deploy to GitHub Pages

```bash
git init
git add index.html seagull.png README.md
git commit -m "Seagull Hunt game"
gh repo create seagull-hunt --public --source=. --push
```

Then on GitHub: **Settings → Pages → Source: Deploy from a branch → main / (root)**.
Your game will be live at `https://<your-username>.github.io/seagull-hunt/` —
open that URL on your phone and play!

Everything is a single self-contained HTML file (no build step, no dependencies),
so it works on any static host: GitHub Pages, Netlify, Vercel, Cloudflare Pages, etc.
