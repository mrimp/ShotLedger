# Release checklist — v2.2.6

## Freeze steps (recommended)
```bash
git init
git add -A
git commit -m "ShotLedger v2.2.6"
git branch -M main
git tag -a v2.2.6 -m "ShotLedger v2.2.6"
git remote add origin <your-repo-url>
git push -u origin main --tags
```

## GitHub Pages
1. Push to GitHub
2. Repo Settings → Pages → Deploy from branch → `main` / `(root)`
3. Ensure `index.html` is the Pages entry point (it redirects to `ShotLedger_Latest.html`)

## Smoke test (before tagging)
- Import ShotMarker CSV with multiple targets
- Import multiple Garmin files (verify mapping UI)
- Import optional Kestrel CSV (verify columns appear)
- Import AMP CSV (verify pill + join health shows)
- Export JSON and re-import JSON (round-trip)
- Exclude a shot (ensure row stays visible + grayed)
- Click Reset / Reset options after sorting or changing density
