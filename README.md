# 🛍️ Customer Spending Analysis Dashboard

**Goal:**  
Perform real-world customer and revenue analysis using the **UCI Online Retail II dataset**, exploring transaction trends, identifying top-performing products and regions, and segmenting customers through **RFM (Recency, Frequency, Monetary)** modeling.

---

## 📊 Project Overview

This project demonstrates an **end-to-end data analysis pipeline** — from cleaning raw transactional data to deriving actionable insights and visualizing them interactively.  
It mirrors the kind of analysis performed in e-commerce and marketing analytics teams.

### Key Highlights
- Processed **400 K+ real transactions** from a UK-based online retailer (2010–2011).  
- Built RFM-based **customer segmentation model** to classify buyers into *Champions, Loyal, Potential Loyalists, At Risk,* and *Lost* groups.  
- Generated interactive dashboards for **monthly revenue trends, top countries, and top products** using Plotly Express.  
- Exported structured outputs for potential use in Tableau/Power BI dashboards.

---

## 🧠 Analytical Workflow

| Phase | Description |
|:--|:--|
| **1. Data Cleaning** | Removed missing `Customer ID`s, canceled invoices (`Invoice` starting with “C”), and negative quantities. |
| **2. Feature Engineering** | Added `Revenue = Quantity × UnitPrice`, and extracted `Year`, `Month`, `DayOfWeek`. |
| **3. Exploratory Analysis** | Identified monthly and country-level revenue drivers. |
| **4. Customer Segmentation (RFM)** | Computed recency, frequency, and monetary values per customer. |
| **5. Scoring & Visualization** | Assigned R/F/M scores (1–5) → Total RFM Score → Customer Segment; visualized distributions. |

---

## 📈 Key Insights

- **Champions + Loyal Customers = ~55 %** of total revenue.  
- **Top 10 products** (home-decor items) generated > 20 % of overall sales.  
- Revenue peaks observed in **Q4 (holiday season)**.  
- Customers with **short recency < 30 days** and **high frequency > 5** show the highest lifetime value.

---

## 🧰 Tech Stack

**Languages & Libraries**  
`Python 3.10` · `Pandas` · `NumPy` · `Matplotlib` · `Seaborn` · `Plotly Express` · `Jupyter`

---

## 🗂️ Folder Structure
```
customer_spending_analysis/
├── data/
│   └── online_retail_II.xlsx 
├── notebooks/
│   └── 01_customer_spending_analysis.ipynb
├── outputs/
│   ├── customer_rfm_summary.csv
│   └── segment_revenue.csv
├── requirements.txt
└── README.md
```


---

## 📎 Data Source
> **Online Retail II Dataset — UCI Machine Learning Repository**  
> [https://archive.ics.uci.edu/ml/datasets/online+retail+ii](https://archive.ics.uci.edu/ml/datasets/online+retail+ii)


---

## 💡 Next Steps
- Deploy as an **interactive Streamlit dashboard**.  
- Extend RFM analysis with **K-Means clustering** for behavior prediction.  
- Integrate with **Supabase / AWS Athena** for large-scale queries.

---

## 📜 License
This project uses the UCI dataset for educational and portfolio purposes only.
