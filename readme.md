# 🎮 Tabletop Game Counter

A mobile-friendly two-player score tracker for card and tabletop games, inspired by the Star Realms aesthetic. Designed to sit on the table between two players.

## Features

- **Two-player split screen** — Player 1 is flipped upside down for the person sitting across the table
- **Score tracking** — Large +/− buttons for easy tapping mid-game
- **Settings menu** — Adjust starting points and roll dice without leaving the game
- **Dice roller** — Rolls a d6 for both players simultaneously, colour-coded blue (P1) and red (P2)
- **Reset with confirmation** — Prevents accidental resets
- **Remembers the game** — Scores and starting points survive a reload or closing the app
- **PWA support** — Install to your home screen and use like a native app
- **Works offline** — No internet required after first load

## Getting Started

### Run locally
Just open `index.html` in a browser. No build step, no dependencies.

### Host on GitHub Pages
1. Push the repo to GitHub
2. Go to **Settings → Pages**
3. Set source to `main` branch, root folder
4. Your app will be live at `https://<your-username>.github.io/<repo-name>/`

### Install as app on mobile (PWA)
Once hosted, open the URL in Safari (iOS) or Chrome (Android):
- **iOS:** tap the Share button → *Add to Home Screen*
- **Android:** tap the browser menu → *Install App* or *Add to Home Screen*

## File Structure

```
tabletop-counter/
├── index.html       ← The entire app
├── manifest.json    ← PWA manifest (name, icons, theme)
├── sw.js            ← Service worker for offline support
└── README.md        ← This file
```

## Customisation

All styling is in the `<style>` block in `index.html`. Key variables to tweak:

| What | Where |
|------|-------|
| Starting points | Change `let startLife = 30;` in the script |
| Player 1 colour (blue) | Search `#00aaff` |
| Player 2 colour (red) | Search `#ff4422` |
| Score font size | `.score { font-size: clamp(...) }` |

## License

MIT — free to use and modify.
