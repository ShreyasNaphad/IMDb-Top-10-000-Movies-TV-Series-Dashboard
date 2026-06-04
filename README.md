# IMDb Top 10,000 Movies & TV Series Dashboard

A pixel-perfect, interactive data visualization dashboard for exploring the top IMDb titles. This dashboard was built purely using HTML, CSS, and JavaScript, with no build steps required.

## Features
- **Zero Dependencies/Build Steps**: Built with pure HTML/CSS/Vanilla JS.
- **Client-Side Data Loading**: Uses [PapaParse](https://www.papaparse.com/) to load and parse the CSV dataset on the fly.
- **Interactive Charts**: Powered by [Chart.js](https://www.chartjs.org/) for Scatter Plots and CSS-based horizontal bar charts mapped to a Viridis color scale.
- **Dynamic Filtering**: Multi-select dropdowns for title types, genre chips, dual-thumb range sliders for years, and minimum vote thresholds.
- **Interactive Data Table**: Sortable, paginated data table with CSV and JSON export functionality.
- **Cinematic Dark Theme**: Custom UI controls matching the provided design system without any default white backgrounds.

## How to Run Locally

Since the dashboard fetches a local CSV file (`title.combined.csv`), you need to serve the directory using a local web server to avoid CORS (Cross-Origin Resource Sharing) issues with `file://` protocol.

### Using Python (Recommended)
If you have Python installed, you can easily start a local server:

```bash
# Python 3
python -m http.server 8080
```
Then, open your browser and navigate to: `http://localhost:8080/index.html`

### Using Node.js
If you have Node.js installed, you can use `http-server` or `serve`:
```bash
npx http-server -p 8080
```
Then, navigate to `http://localhost:8080/index.html`

## Repository Structure
- `index.html`: The main dashboard containing all HTML, CSS styling, and JavaScript logic.
- `title.combined.csv`: The IMDb dataset containing top ranked titles.

## Modifying the Dashboard
Everything is contained within `index.html`. 
- **Styles**: Located in the `<style>` tag, utilizing CSS variables for theming.
- **Logic**: Located in the `<script>` tag at the bottom, handling data loading, filtering state, charts, and the data table.
- **Data**: To use a different dataset, replace `title.combined.csv` and ensure the columns match the logic in the `Papa.parse` block.
