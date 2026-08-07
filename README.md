[README_v0.39.1.md](https://github.com/user-attachments/files/30811915/README_v0.39.1.md)
# Mosaic

*A Meadow Works Studio product.*

Mosaic is a songwriter's idea notebook --- a place where riffs, lyrics,
chords, tabs, audio, and video ideas can live before they become songs.
Instead of asking **"what are you writing?"**, Mosaic asks **"what have
you already created?"** and helps musicians capture, organize,
rediscover, connect, and develop the ideas they already have.

This repository contains the working Mosaic prototype. It is still
intentionally lightweight --- a single-file, mobile-first web app ---
but it has grown well beyond the original clickable simulation. The
current prototype includes real local persistence, media capture and
storage, song workspaces, organization tools, Rediscover,
backup/restore, and portable idea export.

------------------------------------------------------------------------

## Current status

**Current release: v0.39.1 --- Brand Consistency**

Mosaic remains a prototype, but much of the core experience is now
functional.

### Core experience

  -----------------------------------------------------------------------
  Feature                             Status
  ----------------------------------- -----------------------------------
  Audio capture                       ✅ Functional recording and local
                                      media storage

  Video capture                       ✅ Functional recording and local
                                      media storage

  Lyrics capture                      ✅ Real text input and editing

  Chords capture                      ✅ Chord entry, editing, and
                                      reorderable chord chips

  Tab capture                         ✅ Real tab entry and editing

  Idea Detail                         ✅ View and edit captured ideas

  Favorites                           ✅ Supported

  Custom tags / mood tags             ✅ Supported

  Search                              ✅ Supported

  Filter & Sort                       ✅ Supported

  Song Workspace                      ✅ Functional song organization
                                      workspace

  Rediscover                          ✅ Surfaces ideas for creative
                                      rediscovery

  Local persistence                   ✅ Ideas and app state persist
                                      locally

  Media persistence                   ✅ Audio/video stored locally with
                                      IndexedDB

  Backup & Restore                    ✅ Full Mosaic backup and import
                                      workflow

  Library health tools                ✅ Available for checking stored
                                      library/media state

  Single Idea Export                  ✅ Export an individual idea in a
                                      portable format

  Multi-select Export                 ✅ Select and export multiple ideas
                                      together

  Export All Ideas                    ✅ Export the full idea library as
                                      a ZIP

  Accounts / cloud backend            ⬜ Not implemented

  Cross-device sync                   ⬜ Not implemented

  AI-assisted idea matching           🧭 Future direction / exploration
  -----------------------------------------------------------------------

### Idea export

Mosaic distinguishes between **backup** and **export**:

-   **Backup** is intended for restoring Mosaic and preserving the
    complete app state.
-   **Export** is intended for getting creative work out of Mosaic in
    useful, human-readable files.

Bulk exports are created locally in the browser as a ZIP archive.
Depending on the idea type, exports can include readable metadata,
lyrics, chords, tabs, and the original stored audio/video recording when
available.

------------------------------------------------------------------------

## Viewing it

The prototype is currently a single self-contained file:
**`index.html`**. There is no build step and no package installation
required.

-   **GitHub Pages:** visit the Pages URL for this repository if Pages
    is enabled.
-   **Locally:** open `index.html` directly in a modern browser.

Mosaic is designed mobile-first. On a phone-sized screen it fills the
viewport like an app; on desktop it is presented in a phone-style frame
for convenient testing.

> **Important:** Mosaic currently stores data locally in the browser.
> Clearing browser/site storage can remove local data. Use Mosaic's
> backup/export tools to protect important work.

------------------------------------------------------------------------

## Tech notes

-   Plain HTML, CSS, and vanilla JavaScript
-   No framework or build tooling yet
-   Local app state is persisted in browser storage
-   Audio/video media is stored locally using IndexedDB
-   Fonts (Fraunces and Inter) load from Google Fonts via CDN
-   Pointer Events support touch/mouse interactions such as chord
    reordering
-   Backup/restore preserves Mosaic data and stored media
-   Bulk idea export builds a ZIP locally in the browser; creative
    content is not uploaded to a third-party export service

The current single-file architecture is deliberate: it allows the
product experience to evolve quickly while Mosaic is still being
discovered. A future React/TypeScript migration can happen when the
prototype reaches a point where modularization provides more value than
rapid iteration.

------------------------------------------------------------------------

## Product direction

Mosaic is not intended to replace a DAW or generate music for the
songwriter. Its focus is the creative material that often exists
**before** a finished song:

1.  **Capture** an idea quickly.
2.  **Organize** it without creating unnecessary friction.
3.  **Rediscover** ideas that may otherwise be forgotten.
4.  **Connect** ideas that could belong together.
5.  **Develop** those pieces into songs.
6.  **Export** the musician's work whenever they want it.

A longer-term direction is intelligent musical connection: combining
musician-provided context such as tags, mood, chords, key, tempo, or
tuning with audio analysis to help surface ideas that may sound good
together. The goal is not for AI to write the song --- it is for Mosaic
to help musicians remember and reconnect with their own creativity.

------------------------------------------------------------------------

## Folder structure

``` text
mosaic/
├── index.html          ← current working prototype / GitHub Pages entry point
├── README.md           ← project overview
└── brand/
    ├── Meadow-Works-Brand-Reference.docx
    └── Meadow_Works_Logo_Mockups.png
```

------------------------------------------------------------------------

## Brand

Mosaic follows the **Meadow Works Studio** brand system. See
[`brand/Meadow-Works-Brand-Reference.docx`](./brand/Meadow-Works-Brand-Reference.docx)
for the logo usage, color palette, and typography reference.

  Color     Hex
  --------- -----------
  Forest    `#1F3A2E`
  Meadow    `#6D8467`
  Harvest   `#C59D52`
  Cream     `#F4F1E8`
  Slate     `#4A4A4A`

------------------------------------------------------------------------

## Data ownership

A core Mosaic principle is simple:

**Your ideas belong to you.**

Mosaic should make it easy to protect, restore, and export the creative
work entrusted to it. Backup and export features are part of the product
foundation, not an afterthought.

------------------------------------------------------------------------

## Release history

Mosaic maintains release notes and a version history as the prototype
evolves. The current release is **v0.39.1 --- Brand Consistency**, which
standardizes company references as **Meadow Works Studio** while
retaining the Idea Export functionality introduced in v0.39.0.

------------------------------------------------------------------------

*Every idea deserves room to grow.*
