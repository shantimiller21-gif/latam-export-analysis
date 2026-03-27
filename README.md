# LATAM Export Analysis — Panama Canal & Logistics Performance

## Research Question
How does logistics performance and geographic proximity to the Panama Canal 
impact export values in Latin America and the Caribbean?

## Key Findings
- **Timeliness** is the strongest predictor of export value (correlation: 0.44)
- **Canal proximity alone does not predict exports** — Mexico and Brazil are 
  the furthest countries yet dominate regional exports
- **Panama** has the highest LPI score in the region but exports the least, 
  demonstrating that economic scale matters more than logistics quality alone
- **Customs efficiency** is the weakest link across LATAM (correlation: 0.06)

## Tools & Technologies
- Python (pandas, numpy, matplotlib, seaborn, plotly)
- Jupyter Notebook
- Tableau Desktop
- Git & GitHub

## Data Sources
- [World Bank Logistics Performance Index (LPI)](https://databank.worldbank.org/source/logistics-performance-index)
- [UN Comtrade Export Data](https://comtradeplus.un.org)

## Project Structure
```
latam-export-analysis/
├── data/
│   ├── data:world_bank_lpi_latam_caribbean.csv
│   ├── TradeData_3_24_2026_14_26_5.csv
│   └── merged_clean.csv
├── notebooks/
│   └── latam_export_analysis.ipynb
├── visuals/
│   ├── correlation_heatmap.png
│   ├── scatter_distance_exports.html
│   └── choropleth_map.html
└── README.md
```

## Methodology
1. Loaded and cleaned World Bank LPI data for 25 LATAM countries
2. Loaded UN Comtrade export data for 9 LATAM countries
3. Filtered to matching years (2018 & 2022) and merged datasets
4. Calculated geographic distance from each country to the Panama Canal 
   using the Haversine formula
5. Ran correlation analysis across all key variables
6. Built interactive visualizations using plotly and seaborn

## Visualizations
- **Correlation Heatmap** — relationship between logistics factors and exports
- **Scatter Plot** — canal distance vs export value by country
- **Choropleth Map** — regional export performance across LATAM

## How to Run
```bash
git clone https://github.com/shantimiller21-gif/latam-export-analysis.git
cd latam-export-analysis
pip3 install pandas numpy matplotlib seaborn plotly jupyter
jupyter notebook
```
Open `notebooks/latam_export_analysis.ipynb` and run all cells.

## Author
Ashanti Miller | Data Analytics Portfolio Project# LATAM Export Analysis
