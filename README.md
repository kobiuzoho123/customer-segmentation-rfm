# Customer Segmentation & Sales Analysis (Python)

Analysis of 1M+ transactions from a UK online gift retailer (Dec 2009 – Dec 2011) to find out who the most valuable customers are and where revenue comes from.

## Key Findings
- **Champions are 25% of customers but generate 69% of revenue.** Champions and Loyal customers together are 46% of customers and 84% of revenue.
- **825 "At Risk" customers** used to order frequently but haven't bought in about a year. They represent **£1.6M** in past revenue, the biggest win-back opportunity.
- **Strong seasonality:** revenue peaks every November. The best month (Nov 2010, £1.17M) was about 2.6 times the slowest (Feb 2011).
- **82.8% of revenue comes from the UK.** Ireland, the Netherlands and Germany are the top international markets.
- **Top product:** Regency Cakestand 3 Tier (£277,656).

## Process
1. **Data cleaning:** reduced 1,067,371 rows to 779,425 by removing cancelled orders, rows without a customer ID (about 23% of the data), invalid quantities and prices, and duplicates.
2. **Exploratory analysis:** monthly revenue trend, top products (excluding postage and fee codes), and revenue by country.
3. **RFM segmentation:** scored 5,878 customers on Recency, Frequency and Monetary value (quintiles, 1–5) and grouped them into Champions, Loyal, New / Promising, At Risk, Needs Attention and Lost.

## Recommendations
- Protect Champions with loyalty perks and early access to seasonal stock.
- Run a win-back campaign for At Risk customers before the autumn peak.
- Encourage repeat purchases from New / Promising customers.
- Keep spending on Lost customers low.
- Improve customer-ID capture at checkout.

## Tools
Python, pandas, matplotlib, Jupyter Notebook, VS Code

## Data
[Online Retail II](https://archive.ics.uci.edu/dataset/502/online+retail+ii), UCI Machine Learning Repository. To run the notebook, download the dataset into a `data/` folder and install the libraries with `pip install -r requirements.txt`.