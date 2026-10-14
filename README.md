# RetailPulse — Retail Analytics & Demand Insights

Portfolio prototype for the Zidio RetailPulse project using **synthetic demo data**.

## Files
- `sales.csv`: transaction-level retail sales (6,500 orders)
- `customers.csv`: customer attributes (500 customers)
- `products.csv`: product catalogue and unit costs (50 products)
- `inventory.csv`: current stock, lead time and reorder level
- `app.py`: Streamlit analytics dashboard
- `requirements.txt`: Python dependencies

## Run locally
1. Install Python 3.10+.
2. Extract this folder.
3. Open a terminal in this folder and run:
   ```bash
   pip install -r requirements.txt
   streamlit run app.py
   ```
4. Open the local URL Streamlit prints in the terminal.

## Features
- KPI summary, monthly trend, category and regional sales
- RFM customer segmentation using K-Means
- Baseline 30-day demand forecast and holdout MAPE
- Simple churn-risk classifier with feature importance
- Inventory reorder recommendations
- Filtered sales CSV download

## Important limitations
- All data is synthetic and created for practice.
- Forecasting uses a simple 7-day-average baseline, not Prophet/LSTM.
- Churn is a proxy label (no purchase in the final 90 days of the dataset); it is not verified customer churn.
- Cluster numbers are arbitrary IDs and should be interpreted from their RFM profiles.
- The dashboard is a local prototype until you deploy it.
- Do not report the project’s target business impact as measured results. Report only metrics calculated by your implementation.

## Suggested next steps
1. Inspect data quality and document assumptions.
2. Compare the baseline forecast with a second model.
3. Add a time-based validation strategy for churn.
4. Add tests, screenshots, a project report and a demo video.
