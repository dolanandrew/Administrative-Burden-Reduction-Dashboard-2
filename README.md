# Administrative-Burden-Reduction-Dashboard-2
Dashboard identifying targets for executive branch administrative burden reduction, including program, administering agency, and estimated annual hours saved.

## Viewing the dashboard

Publish this repository with GitHub Pages and visit its Pages URL. To view it locally, run `python3 -m http.server` from the repository root and open `http://localhost:8000/`. The page loads D3.js from a CDN, so an internet connection is required.

The dashboard uses federal information collection request (ICR) data from [reginfo.gov](https://www.reginfo.gov/public/do/PRAMain), compiled in November 2026. `burden_reductions.csv` contains collections whose annual paperwork burden fell by at least 75,000 hours.
