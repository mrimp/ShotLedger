# ShotLedger — v1.6-FINAL

Single-file, fully offline HTML app to merge **ShotMarker** targets with **chrono (Garmin)**, optional **Kestrel** weather logs, and optional **AMP** traces — then review shots, flags, and per-target summaries.

## Quick start
1. Download the repo ZIP and unzip.
2. Open `index.html` in a desktop browser (Chrome/Edge recommended).
3. Import your files:
   - ShotMarker CSV (multi-target)
   - Chrono files (one per target/string; mapping UI handles ordering mistakes)
   - Optional: Kestrel CSV
   - Optional: AMP CSV
4. Pair chrono ↔ target (dropdowns) if needed.
5. Review:
   - Target headers include **join health** (G/K/A coverage on record shots)
   - Per-target mini baselines (avg vel, ES/SD, etc.)
   - Per-shot flags and notes

## What’s in this release (v1.6-FINAL)
- Join health in the target header (Garmin/Kestrel/AMP coverage)
- Per-target baselines in the rollup bar
- AMP rendered as an import pill (no leftover status text)
- Notes UI toned down (dark theme aligned)
- Extra spacing below chart/table region
- Table sorting + **Reset Defaults** button

## Data & privacy
Everything runs locally in your browser. No network calls, no telemetry.

## GitHub Pages
This repo is already Pages-ready because the app is `index.html`.

- Settings → Pages → Deploy from branch → `main` / `(root)`
- After it publishes, you can load the app from the Pages URL.

## Support / bugs
If something looks off, grab a screenshot + the browser console error (if any) and open an issue.
