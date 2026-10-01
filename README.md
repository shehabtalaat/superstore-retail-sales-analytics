# superstore-retail-sales-analytics
End-to-End Retail Data Analytics &amp; EDA on Sample Superstore dataset using Python, featuring RFM Customer Segmentation, Feature Engineering, and Strategic Profitability Analysis.
# 📊 Retail Performance & Sales Analytics Project

An end-to-end data analytics and exploratory data analysis (EDA) project on the **Sample Superstore** dataset using Python. This project evaluates retail performance, pinpoints the root causes of financial loss (margin leakage), and segments customer value using an RFM model to deliver data-driven business strategies.
---
## 📌 Project Overview
The objective of this project is to clean, transform, and analyze historical retail sales transactions across the United States. Through deep exploratory analysis and feature engineering, the project identifies operational inefficiencies and strategic discounting thresholds to protect profit margins without harming revenue growth.
---
## 🎯 Key Objectives
- **Data Cleaning & Pipeline Architecture:** Built reusable Python functions to handle missing values (Postal Code imputation), eliminate duplicate rows, and cast correct data types.
- **Feature Engineering:** Derived temporal, financial, and operational metrics (`Shipping_Days`, `Profit_Margin`, `Unit_Price`, `Discount_Amount`, `Discount_Bracket`, `Is_Loss`).
- **Exploratory Data Analysis (EDA):** Evaluated distributions, outlier bounds using the Interquartile Range (IQR) method, and numerical correlations.
- **Customer Segmentation (RFM):** Modeled Recency, Frequency, and Monetary scores to segment customers into actionable tiers (A, B, C, D).
- **Strategic Business Questions:** Answered key questions regarding product categories, shipping modes, seasonality, and regional profitability.
---
## 🛠️ Tech Stack & Libraries
- **Language:** Python
- **Data Manipulation & Analysis:** `pandas`, `numpy`, `pyarrow`
- **Data Visualization:** `matplotlib`, `seaborn`
- **Environment:** Jupyter Notebook
---
## 📂 Project Structure
```text
├── Sample-Superstore2019.csv            # Raw dataset
├── Sample-Superstore2019_cleaned.csv    # Cleaned dataset (CSV)
├── Sample_Superstore_2019_Clean.parquet # Cleaned dataset (Parquet format)
├── Mini_Project.ipynb                   # End-to-End Jupyter Notebook
└── README.md                            # Project documentation & summary

🔍 Key Findings & Analytical Highlights
1. The Impact of Discounting (Margin Destruction)
Strong Negative Correlation: A correlation of -0.86 between Discount and Profit_Margin indicates that aggressive discounting severely destroys bottom-line profitability.

Loss Escalation: Correlation between Discount and Is_Loss reached +0.75. Transactions with discounts exceeding 20% consistently generate aggregate losses:

No Discount (0%): 0% loss rate, ~34% average profit margin.

Medium Discount (21-50%): 91.6% loss rate, -22% average margin.

High Discount (>50%): 100% loss rate, -113.8% average margin.

2. Product Sub-Category Performance
Top Profit Generators: Copiers (+$55.6k profit, 0% loss rate), Phones (+$44.5k), and Accessories (+$41.9k).

Financial Leakage Areas: Tables (-$17.7k total loss, 63.6% loss rate) and Bookcases (-$3.4k loss, 47.8% loss rate) suffer major financial deficits caused primarily by deep discounting strategies.

3. Customer Segmentation (RFM Analysis)
Segment A (Champions / VIPs): High monetary value (~$4,773 avg spend) and low recency (~37 days). High priority for loyalty retention.

Segment B (Potential Loyalists): Frequent buyers with solid spending; prime targets for upsell and cross-sell campaigns.

Segment C (Needs Attention): Moderate spending and recency; suited for automated re-engagement workflows.

Segment D (At-Risk / Inactive): Lowest frequency and recency (>317 days); recommended for win-back campaigns or reduced acquisition spend.

💡 Strategic Recommendations
Enforce Strict Discount Caps: Cap promotional discounts at 20% across vulnerable sub-categories (Tables, Bookcases, Supplies) to immediately stop negative margins.

Promote High-Margin Anchors: Focus marketing spend on top performers such as Copiers, Phones, and Paper.

Logistics Optimization: Re-evaluate pricing on standard shipping classes where volume is high but margin capture is lower compared to second-class fulfillment.

Targeted Retention: Allocate dedicated account management to RFM Segment A customers to maximize Customer Lifetime Value (CLV).

👤 Author
Shehab Talaat Ismail

Role: Data Analyst
