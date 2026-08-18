# 💰 500K Challenge

A mobile-first Progressive Web App (PWA) that helps you save ₦500,000 by a target date — one day (or week) at a time.

**Live demo:** https://500ksavgoal.netlify.app

![500K Challenge screenshot](icon-512.png)

## Features

- 🎯 Daily or weekly savings tracking, toggle anytime
- 📊 Live progress bar and total-saved counter
- 🔥 Streak tracking and a full month calendar view
- 📈 Projected finish date based on your actual saving pace
- 🎉 Milestone celebrations (confetti) at 25%, 50%, 75%, and 100%
- ✏️ Log a custom amount or edit/undo a mistaken entry
- 🧮 Built-in goal calculator — enter any target amount and date, get the required daily/weekly/monthly savings
- 🔔 In-app reminder notifications that stop automatically once you've saved for the day
- 🌗 Dark mode
- 💾 Export/import your data as a backup file
- 📲 Installable as a home screen app, works fully offline

## Tech

Vanilla HTML, CSS, and JavaScript — no frameworks, no build step. Data is stored in the browser's `localStorage`. Offline support and installability are handled with a `manifest.json` and a `sw.js` service worker.

## Run locally

Clone the repo and open `index.html` in a browser, or serve it with any static file server:

```bash
npx serve .
```

Note: the service worker and "Add to Home Screen" prompt only work when served over `https://` or `localhost` — opening `index.html` directly as a file won't enable offline mode or installability.

## Project structure

```
├── index.html      # App markup, styles, and logic
├── manifest.json    # PWA manifest (name, icons, theme color)
├── sw.js            # Service worker for offline caching
├── icon-192.png      # App icon (192x192)
└── icon-512.png      # App icon (512x512)
```

## Author

Zuokemefa Oyinmiebi Peter — built while learning software development at Learn2earn.
