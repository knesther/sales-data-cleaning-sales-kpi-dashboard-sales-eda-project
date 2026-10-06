# sales-data-cleaning-sales-kpi-dashboard-sales-eda-project
End‑to‑end workflow for sales data cleaning, recovery audit, validation, KPI scorecard, and visualization in Python.
# 📊 Sales Data Cleaning & KPI Dashboard

## 📌 Project Overview
This project demonstrates a complete **data pipeline** for sales analysis:
- Raw sales data → Cleaning → Missing Data Recovery → Validation → KPI → Visualization.
- Ensures **no visualization is produced from unresolved raw-data defects** without first documenting them.

## 🛠 Workflow
1. **Data Cleaning & Standardization**  
   - Converted text to numeric values, standardized labels, removed duplicates.  
2. **Missing Data Recovery Audit**  
   - High-confidence recovery using business rules (e.g., Sales = Quantity × Unit Price × (1-Discount)).  
   - Unresolved values documented transparently.  
3. **Validation Checklist**  
   - PASS for duplicates, Order_ID uniqueness, numeric ranges, and business rules.  
4. **KPI Scorecard**  
   - Headline metrics for orders, units, sales, profit, margin, discounts.  
5. **Visualizations**  
   - Monthly trend, Region, Category, Product, Salesperson, Discount impact.

## 📦 Deliverables
- `Sales_Data_Cleaned.csv` → analysis-ready dataset.  
- **Recovery Audit** → transparent record of recovered vs unresolved values.  
- **Validation Results** → structural and business-rule checks.  
- **KPI & Visualization Dashboard** → insights into sales performance.

## 📈 KPI Highlights
- **Total Orders:** 119  
- **Units Sold:** 318  
- **Total Sales:** ₹ 4,512.78 Lakh  
- **Total Profit:** ₹ 726.12 Lakh  
- **Profit Margin:** 16.1%  
- **Average Order Value:** ₹ 37,930  
- **Average Units per Order:** 2.7  
- **Biggest Single Order:** ₹ 496,000  
- **Average Discount:** 10.2%  

*(Values based on `Sales_Data_Cleaned.csv`)*

## 📊 Visual Storytelling
1. **Monthly Sales by Category** – stacked bar chart showing category contribution each month.  
2. **Sales by Region** – bar chart comparing regional performance.  
3. **Sales vs Profit by Category** – side-by-side bars highlighting profitability.  
4. **Units Sold by Product** – bar chart showing product demand.  
5. **Sales by Salesperson** – bar chart ranking salesperson contribution.  
6. **Discount vs Sales Scatterplot** – shows how discounts relate to sales volume.

## 🔑 Key Insights
- **Regional performance:** North and South drive the majority of sales.  
- **Category profitability:** Electronics dominate revenue, Accessories show steady margins.  
- **Product demand:** Tablets and Smartphones lead in units sold.  
- **Salesperson impact:** Clear differences in contribution, with top sellers driving large orders.  
- **Discount effect:** Higher discounts don’t always lead to higher sales — margins drop at higher discounts.

## 🚀 How to Run
```bash
pip install pandas matplotlib seaborn
jupyter notebook Sales_Data_EDA.ipynb

