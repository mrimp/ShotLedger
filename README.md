# ShotLedger — v2.3.0

ShotLedger is a **single-file, offline HTML** tool for pairing ShotMarker + Chrono/Garmin (+ optional Kestrel/AMP) and reviewing your strings fast.

**Live (GitHub Pages):** https://mrimp.github.io/ShotLedger/

## Quick start
- **Web:** open the GitHub Pages link above (or `index.html` in the repo root).
- **Offline:** download the repo and open `ShotLedger_Latest.html` directly in your browser.

## Files
- `index.html` → redirects to the latest build (GitHub Pages entry point)
- `ShotLedger_Latest.html` → the current single‑file app (offline)
- `releases/` → pinned release builds

## Notes
- Designed to work **offline** (no external JS/CSS, no CDNs).
- Excluding a shot **keeps the row visible** and grays it out (non-destructive).
- “Reset” is wired to restore the table view and preferences.

## License
See `LICENSE`.
