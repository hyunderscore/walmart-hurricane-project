# Walmart Hurricane Analytics

DS2002 Fall 2026 midterm project by Andrew and Anh.

## Team

| Name | GitHub | Role |
|------|--------|------|
| Andrew | [@hyunderscore](https://github.com/hyunderscore) | Cleaning and decision log |
| Anh | [@anhnbach](https://github.com/anhnbach) | Weather API and joins |

## Project purpose

This project analyzes Walmart transaction, product, store, distribution-center,
inventory, and weather data to identify hurricane-related demand changes.

## Summary

We cleaned 25,562 transaction rows down to 24,521 and merged 45 SKUs into 20 products. Breakfast sales rose 415% and Emergency sales rose 186% in the week before landfall, and all 12 stores surged at about the same time.

## Questions answered

1. Which categories experienced the largest demand surge?
2. How does SKU consolidation change the Pop-Tarts analysis?
3. How are weather conditions related to sales?
4. Do stores show different geographic surge patterns?
5. Is the Entertainment increase a real signal or a data artifact?

## Data

| File | Notes |
|------|-------|
| `walmart_transactions.csv` | Sales transactions |
| `store_locations.csv` | Store info |
| `product_catalog.csv` | Product and SKU info |
| `distribution_centers.csv` | Distribution center info |
| `inventory_and_sales.db` | SQLite database used in Question 5 |

Weather API: Open-Meteo, base URL `https://archive-api.open-meteo.com/v1/archive`

## Repository structure

- `data/` contains the CSV and SQLite data files.
- `notebooks/team_notebook.ipynb` contains the complete analysis.
- `CHARTER.md` contains the team responsibilities and workflow.

## Requirements

Python 3 with:

- pandas
- matplotlib
- seaborn
- requests
- jupyter

## How to run

1. Clone this repo.
2. Install the packages: `pip install pandas matplotlib seaborn requests jupyter`
3. Open `notebooks/team_notebook.ipynb` and run Restart and Run All. The weather cell needs internet to reach Open-Meteo.

In Colab, first run `!git clone https://github.com/hyunderscore/walmart-hurricane-project.git` and `%cd walmart-hurricane-project/notebooks` so the data files load.

## Key findings

- Breakfast rose the most, from 73 to 377 units a day, a 415% increase.
- Pop-Tarts peaked at 678 units a day once its 4 SKUs were combined. No single SKU went above 240.
- Wind speed had the strongest correlation with sales, 0.47 across 30 days, with about a 2-day lag.
- All 12 stores surged 2.2x to 2.8x, so the surge was statewide.
- The +250% for board games was only one day. The full week was +135%.

## Recommendation

Stock all 12 stores before landfall, not just the ones near the path, and plan for about 5x normal Breakfast and 3x Emergency. Stock extra board games, but plan for a little over 2x for the week.

## Reflection

The reflection answers are at the end of `notebooks/team_notebook.ipynb`.