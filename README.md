# Superstore Executive Dashboard

An interactive, single-file HTML dashboard built for executive-level reporting on US retail performance

🔗 Live Dashboard: (https://mohim-khan.github.io/superstore-executive-dashboard/Superstore_Dashboard.html)

## What it covers

- **4 years of transaction data** (2018–2021) across US retail operations
- **3 product categories**, **4 regions**, **3 customer segments**, and **17 sub-categories**
- Fully interactive filtering by year, region, segment, category, and ship mode — every chart and KPI updates live
- 10+ charts: monthly sales & profit trend, category revenue split, profit margin by sub-category, regional performance, customer segment growth, sales-vs-profit bubble analysis, discount impact on profit, top revenue states, shipping mode breakdown, and year-over-year growth
- A dynamic insights panel that generates plain-language takeaways as filters change

## Data quality note

During analysis, 11 order lines were found with anomalous $50,000 sales values — well outside the normal $5–$2,000 range for this dataset, and almost certainly data-entry errors. These were identified, excluded, and documented rather than silently included, so all figures shown reflect the cleaned dataset (9,983 order lines / 5,006 distinct orders).

## Tech

- Single self-contained `.html` file — no build step, no backend
- [Chart.js](https://www.chartjs.org/) for all data visualizations, loaded via CDN
- Vanilla JavaScript for filtering, aggregation, and dynamic insight generation
- No external API calls — the full dataset is embedded client-side

## Data source

Based on the classic Superstore retail dataset, cleaned and re-aggregated for this project.
