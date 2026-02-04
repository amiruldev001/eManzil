# eManzil (PWA)

A simple installable offline PWA that shows the Manzil compilation as flashcards.

## Features
- Installable (Add to Home Screen)
- Offline-first (Service Worker caching)
- Flashcard mode (tap to show/hide translation)
- Translation: English / Malay
- Dark/Light mode
- Swipe left/right (mobile)

## How to run locally
Because Service Workers require HTTPS (or localhost), use a simple local server:

### Option 1 (Python)
```bash
python -m http.server 5173
```

Then open:
http://localhost:5173/

### Option 2 (VS Code)
Install extension: **Live Server** and click "Go Live".

## Add the real Manzil verses
Edit:
`data/manzil.json`

Format:
```json
[
  { "surah":"...", "ayah":1, "arabic":"...", "en":"...", "ms":"..." }
]
```

## Deploy (GitHub Pages)
- Push these files to a GitHub repo
- Settings → Pages → Deploy from branch
- Visit your GitHub Pages URL
