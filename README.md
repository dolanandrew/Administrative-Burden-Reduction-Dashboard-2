# Administrative-Burden-Reduction-Dashboard-2
Dashboard identifying targets for executive branch administrative burden reduction, including program, administering agency, and estimated annual hours saved.

## Viewing the dashboard

Publish this repository with GitHub Pages and visit its Pages URL. To view it locally, run `python3 -m http.server` from the repository root and open `http://localhost:8000/`. The page loads D3.js from a CDN, so an internet connection is required.

The dashboard uses federal information collection request (ICR) data from [reginfo.gov](https://www.reginfo.gov/public/do/PRAMain), compiled in November 2026. `burden_reductions.csv` contains collections whose annual paperwork burden fell by at least 75,000 hours.

The page filters the CSV in JavaScript, excluding ICRs with an **Active** status and those whose respondent type is **Organizations**. Requests received in OIRA or preapproved remain eligible, as do requests for individuals, both individuals and organizations, or unspecified respondents. The CSV itself is unchanged; the exclusion lists are constants near the top of the script.

The chart groups ICRs by department or agency in packed-circle panels, sorted by total annual hours saved. Each panel shows its ICR count and total hours saved. Inner circle area represents hours saved on a shared scale across all agencies, and color identifies respondent type. Hover over or focus a circle for details, and select it to open the source on reginfo.gov.
