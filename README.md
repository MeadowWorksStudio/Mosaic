[README.md](https://github.com/user-attachments/files/30364075/README.md)
# Mosaic

*A Meadow Works product.*

Mosaic is a songwriter's idea notebook — a place where riffs, lyrics, and chord ideas live before they become songs. Instead of asking "what are you writing?", Mosaic asks "what have you already created?" and helps you rediscover and connect the ideas you've already captured.

This repo is the working prototype. It's early — a clickable, no-backend simulation of the core experience, built to test whether the concept *feels* right before any real engineering investment.

---

## Current status

**Sprint 1 — Clickable Prototype**

Screens built so far:
- **Splash** — Meadow Works / Mosaic intro
- **Dashboard** — greeting, Continue Working, Recent Ideas, Recent Songs, Connections
- **Capture** — choose Audio, Video, Lyrics, Chords, or Tab
- **Idea Detail** — the "Tile" view for any single idea

What's real vs. placeholder right now:
| Feature | Status |
|---|---|
| Lyrics capture | ✅ Real text input, editable afterward |
| Chords capture | ✅ Real chord entry, reorderable pill chips, editable afterward |
| Audio / Video / Tab capture | 🔶 Placeholder — generates fake sample content, marked "Preview" in the UI |
| Continue Working / Recent Songs | 🔶 Placeholder — not yet wired to real activity |
| Song Workspace | ⬜ Not built yet |
| Persistence | ⬜ None — everything resets on page refresh |
| Accounts / backend | ⬜ None |

Not yet built: real input for Tab, the Song Workspace canvas, and any kind of persistence or backend. Those are the next pieces on deck.

---

## Viewing it

The whole prototype is a single self-contained file: **`index.html`**. No build step, no dependencies to install.

- **On your phone or a browser, right now:** open `index.html` directly, or visit the GitHub Pages link for this repo (once enabled in Settings → Pages).
- **Locally:** just double-click `index.html`, or drag it into any browser.

It's built mobile-first — on a phone-sized screen it fills the whole viewport like a real app; on a desktop browser it shows inside a floating phone-frame mockup for easier viewing.

---

## Tech notes

- Plain HTML, CSS, and vanilla JavaScript — no framework, no build tools.
- All state (ideas, songs, edits) lives in memory only, for this prototype stage. Refreshing the page resets everything.
- Fonts (Fraunces, Inter) load from Google Fonts via CDN.
- Drag-to-reorder (chord chips) uses Pointer Events, so it works the same with a mouse or a real touchscreen.

The plan is for this prototype to inform, not be thrown away — once the experience feels right, it becomes the reference for a real React/TypeScript build.

---

## Folder structure

```
mosaic/
├── index.html          ← the clickable prototype (this is what Pages serves)
├── README.md            ← you are here
└── brand/
    ├── Meadow-Works-Brand-Reference.docx
    └── Meadow_Works_Logo_Mockups.png
```

## Brand

Mosaic follows the Meadow Works brand system — see [`brand/Meadow-Works-Brand-Reference.docx`](./brand/Meadow-Works-Brand-Reference.docx) for the full logo usage, color palette, and typography guidelines.

Quick reference:

| Color | Hex |
|---|---|
| Forest | `#1F3A2E` |
| Meadow | `#6D8467` |
| Harvest | `#C59D52` |
| Cream | `#F4F1E8` |
| Slate | `#4A4A4A` |

---

*Every idea deserves room to grow.*
