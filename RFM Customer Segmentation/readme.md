# RFM Customer Segmentation Analysis
Segmentation of ~5,900 customers from a UK-based online retailer (Dec 2009 – Dec 2011, ~780,000 transactions) using Recency, Frequency, and Monetary (RFM) analysis to identify high-value customers, retention risks, and revenue concentration.

## Tools Used
Python (Pandas, NumPy, Matplotlib) — data cleaning, RFM scoring, segmentation logic.

## Key Insights
Revenue is highly concentrated: Champions and Loyal Customers make up just 46% of the customer base but generate 83.7% of total revenue (£14.5M of £17.4M) — a clear Pareto pattern worth protecting with retention efforts.
Champions alone (25% of customers) drive 69% of revenue ($12M), averaging 15.7 orders per customer and purchasing as recently as 20 days ago on average.
£1.09M in revenue is sitting in the "At Risk" segment — 353 customers who were previously frequent buyers (avg. 7.6 orders) but haven't purchased in 344 days on average. One customer alone (ID 12346) represents £77.5K in historical spend and hasn't ordered in 326 days — a strong win-back campaign candidate.
"Lost" and "Hibernating" segments (25% of customers) contribute under 3% of revenue combined — low priority for retention spend compared to At Risk customers.

## Files
01_data_cleaning.ipynb — data cleaning (removes cancelled orders, missing customer IDs, duplicates)
02_rfm_analysis.ipynb — RFM calculation, scoring, and segmentation logic
03_visualization.ipynb — exploratory visualizations (segment revenue share, recency vs monetary, RF heatmap)
rfm_segments.csv — full customer-level RFM dataset (Power BI data source)
Raw dataset: Online Retail II, UCI Machine Learning Repository (not included here due to file size — see 01_data_cleaning.ipynb for the cleaning steps applied).
