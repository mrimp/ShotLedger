# Release checklist — v1.6-FINAL

## Freeze steps (recommended)
```bash
git init
git add -A
git commit -m "ShotLedger v1.6-FINAL"
git branch -M main
git tag -a v1.6-FINAL -m "ShotLedger v1.6-FINAL"
git remote add origin <your-repo-url>
git push -u origin main --tags
```

## GitHub Pages
1. Push to GitHub
2. Repo Settings → Pages → Deploy from branch → `main` / `(root)`
3. Wait for the Pages URL to appear

## Smoke test (before tagging)
- Import ShotMarker CSV with multiple targets
- Import multiple Garmin files (verify mapping UI)
- Import optional Kestrel CSV (verify columns appear)
- Import AMP CSV (verify pill + join health shows)
- Export JSON and re-import JSON (round-trip)
- Click **Reset Defaults** after sorting
```
