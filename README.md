# Noles in the Show

Tracking FSU Seminoles baseball players in professional baseball — live stats, rosters, and minor league updates.

🌐 **[nolesintheshow.com](https://nolesintheshow.com)**

---

## What It Does

- Pulls current season stats from the MLB Stats API for all players on the Noles in the Show roster
- Updates a live Excel workbook (`noles_in_the_pros.xlsx`) with a "2026 Stats" sheet
- Regenerates a self-contained HTML dashboard (`noles_dashboard.html`) with sortable tables, player cards, and minor league tracking

## Files

| File | Description |
|------|-------------|
| `noles_stats_updater.py` | Main script — fetches stats and regenerates the dashboard |
| `noles_dashboard.html` | Auto-generated live dashboard (do not edit manually) |
| `noles_in_the_pros.xlsx` | Excel workbook with roster and stats |
| `player_id_cache.json` | Caches MLB player ID lookups to reduce API calls |
| `.github/workflows/` | GitHub Actions workflow for scheduled auto-updates |

## Running Locally

```bash
pip install openpyxl requests
python noles_stats_updater.py
```

## Auto-Updates

The dashboard updates automatically via GitHub Actions on a scheduled basis. The latest run status is shown in the repo badge above.

---

*Noles in the Show is a fan site and is not affiliated with Florida State University or Major League Baseball. Data sourced from the MLB Stats API.*
