# ShotLedger (v1.0.0)

A standalone, **in-browser** shot log + analysis tool for F-Class / long-range workflows.

- Imports: **ShotMarker CSV**, **Garmin Chrono CSV/XLS**, **AMP CSV**
- Manual inputs (optional): primer seat, wind/elev zero deltas, wind call, notes
- Deterministic **locked thresholds** for flags (rails-only v1.0)
- Export/Import JSON snapshots (shareable, portable)

> Everything runs locally in your browser. No server, no installs.

---
Run it
Live (GitHub Pages): https://mrimp.github.io/ShotLedger/

## Quick start

1. Open **index.html** (double-click it).
2. Click **ShotMarker CSV** and load your ShotMarker export(s).
3. Optionally load:
   - **Garmin Chrono (multi: CSV/XLS)**
   - **AMP CSV**
4. Use **Export JSON** to save a combined dataset snapshot.

### GitHub Pages (optional)
This repo includes `docs/index.html` so you can host via GitHub Pages:

- Repo → **Settings** → **Pages**
- Source: `Deploy from a branch`
- Branch: `main`
- Folder: `/docs`

---

## Locked thresholds (v1.0.0)

### String-level flags (record shots only)
- **SD (fps)**: OK ≤ 10 • Warn > 10 • Red > 14  
- **ES (fps)**: OK ≤ 30 • Warn > 30 • Red > 40

### Per-shot flags
- **Radial MOA**: OK ≤ 0.30 • Warn 0.30–0.45 • Problem 0.45–0.60 • Red > 0.60  
- **Vertical |MOA|**: Warn > 0.35 • Red > 0.50  
- **Velocity dev from string avg (in SD units)**:  
  OK ≤ 0.5σ • Warn 0.5–1.0σ • Problem 1.0–1.5σ • Red > 1.5σ

---

## Notes

- This v1.0 release is **rails-only**: flags are deterministic from the locked thresholds above.
- Targets/strings are grouped with rollups; **targets start collapsed** for a clean overview.

---

## License
MIT — see [LICENSE](LICENSE).
