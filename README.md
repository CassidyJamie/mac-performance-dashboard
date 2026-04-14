# Mac Performance Dashboard

A self-contained HTML dashboard for tracking Mac weekly sell-through performance vs JST.

## Features
- Upload weekly ag-grid exports (.xlsx) to visualise ST vs JST by product family and country
- Key insights with supply constraint / demand softness signals and JST review recommendations
- Country beats & misses tables with velocity bars — filterable by product
- Country → Product inverse view
- Multi-week trend heatmap (Product Family & By Country views) with streak detection
- Sparklines on product cards
- History stored in browser localStorage (up to 8 weeks)
- Export / Import history as JSON to share with teammates

## Usage
1. Open `index.html` in any modern browser (Chrome, Safari, Firefox)
2. Upload your weekly ag-grid export (.xlsx)
3. Each week's data is saved automatically — no re-upload needed
4. Use **Export weeks (.json)** to share your history with teammates
5. Teammates use **Import weeks (.json)** to load your history

## GitHub Pages
Visit the live dashboard at: https://[your-username].github.io/mac-performance-dashboard

## Sharing data with teammates
To pre-seed the dashboard with your history for all users:
1. Click **Export weeks (.json)** in the dashboard
2. Open `index.html`, find `const PRELOADED_HISTORY = [];`
3. Replace `[]` with the contents of your exported JSON
4. Commit and push — all users who open the page will start with your data
