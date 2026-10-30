LUMETRA — GITHUB PAGES STATIC EDITION

This is a static, browser-only version of Lumetra. No Python, Flask, terminal commands, or backend server are needed.

PUBLISH WITH GITHUB PAGES
1. Open https://github.com and create a new public repository named Lumetra (or use your existing DATAPILOT-AUTONOMOUS repository).
2. Upload index.html to the repository root (not inside a nested folder). Commit the change.
3. Open repository Settings → Pages.
4. Under Build and deployment, choose Deploy from a branch.
5. Select branch main and folder /(root), then Save.
6. Wait for the Pages deployment to finish. Your site will be available at https://YOUR-USERNAME.github.io/REPOSITORY-NAME/.

HOW IT WORKS
- Upload CSV/TSV/TXT or Excel files in the page. Parsing and analysis happen in your browser.
- Includes adaptive light/dark theme, KPI cards, interactive charts, category ranking, a rule-based data analyst, searchable/paginated data explorer, data-quality checks, and Excel report export.
- “Try sample data” loads built-in demo data.
- Libraries are loaded from CDNs, so visitors need an internet connection for Chart.js and Excel import/export.
- Uploaded data is not sent to a server by this static app. Avoid browser extensions or untrusted devices when handling confidential data.

IMPORTANT LIMITATION
GitHub Pages only hosts static files. It cannot run the Flask/Python backend from the previous package. This edition replaces backend-dependent features with in-browser processing, so it can run directly on GitHub Pages. The analyst is rule-based and descriptive, not a connected LLM. It does not support arbitrary AI reasoning, database connections, authentication, or multi-user saved projects.

To update your published site, replace index.html in the repository root and commit the change.


UPDATE NOTES
- Added a quick guide explaining Group by, Measure, and Aggregation in plain language.
- Improved line-chart rendering with visible points, smoother lines, and hover tooltips.
- Fixed line-chart ordering: date labels are sorted chronologically and numeric labels numerically; other categories keep their original data order. Bar charts remain ranked by value.
- For best line-chart results, choose a date/month column as Group by and a numeric field such as sales, revenue, or temperature as Measure.
