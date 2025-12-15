# Banking Customer Analytics Dashboard

End-to-end banking analytics project combining Python exploration with a Power BI dashboard. The goal is to profile customers, understand product uptake, assess risk, and surface actionable insights for banking teams.

## Highlights
- Power BI dashboard for interactive drill-down across customer segments and products.
- Python notebook for quick EDA: distributions, missingness, and data quality checks.
- Clean CSV dataset (~3k rows, 20+ columns) with demographics, products, balances, and risk labels.
- Lightweight, reproducible setup with pinned Python dependencies.

## Repository Layout
- Data/Banking.csv — raw dataset.
- analysis.ipynb — Jupyter notebook for exploratory analysis.
- main.py — placeholder for future automation/scripts.
- requirements.txt — Python dependencies.

## Data Notes
- 3,000+ customer records with demographics (age, location, occupation, gender) and product usage (credit cards, loans, deposits, checking/savings, FX, business lending).
- Financial metrics: estimated income, balances, properties owned, superannuation savings, fee structure.
- Labels include loyalty tier (Jade/Gold/Silver/Platinum) and risk weighting.

## Quickstart (Python)
1) Create a virtual environment (recommended):
   - Windows: `python -m venv .venv && .venv\Scripts\activate`
   - macOS/Linux: `python -m venv .venv && source .venv/bin/activate`
2) Install deps: `pip install -r requirements.txt`
3) Launch notebook: `jupyter notebook analysis.ipynb`

## Quickstart (Power BI)
1) Open the Power BI report file (`Banking Dashboard (2025).pbix` if available) in Power BI Desktop.
2) Ensure the data source points to `Data/Banking.csv`. If prompted, set the file path to this repository location.
3) Refresh the model and interact with the visuals (drill-down, slicers for loyalty tiers, products, regions, and risk levels).

## Notebook Walkthrough
- Load data, inspect schema, and review column summaries.
- Visualize age distribution and key product uptake patterns.
- Check missing values and basic data quality signals before modeling or BI.

## Ideas for Extension
- Churn and cross-sell propensity models using scikit-learn or LightGBM.
- Customer lifetime value estimation segmented by loyalty tier and risk.
- Anomaly and fraud-style monitoring using transaction or balance deltas.
- Automated data refresh scripts in `main.py` to feed the BI model.

## Tech Stack
- Python 3.13, pandas, numpy, matplotlib, seaborn, Jupyter.
- Power BI Desktop for dashboarding.

## Contributing
Issues and pull requests are welcome. Please include a concise description, reproduction steps, and screenshots for dashboard changes when possible.

## License
This project is intended for educational and portfolio use. Add a specific license if you plan to distribute or commercialize.

