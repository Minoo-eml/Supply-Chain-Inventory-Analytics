# Supply Chain & Inventory Analytics

An end-to-end data analytics project focused on **inventory performance, stock risk, demand forecasting, and supplier reliability**.

This project combines **Python for data preparation and analysis** with **Power BI for interactive business visualization**, transforming operational inventory data into actionable supply chain insights.

---

## 📌 Project Overview

Inventory management requires balancing product availability, working capital, demand uncertainty, and supplier performance.

The goal of this project is to analyze inventory data across **1,000 SKUs** and identify:

* Inventory value and stock distribution
* Products at risk of stockout
* Reorder and safety stock risks
* Negative Available-to-Promise (ATP)
* Demand forecast accuracy
* Supplier delivery performance
* Inventory exposure across product categories
* ABC inventory classification

The project follows an end-to-end analytics workflow:

**Raw Data → Data Cleaning → Business Validation → Feature Engineering → KPI Analysis → Power BI Dashboard → Business Insights**

---

## 🎯 Business Problem

A supply chain team needs to answer questions such as:

* How much capital is currently tied up in inventory?
* Which SKUs are approaching stockout risk?
* Which products have negative Available-to-Promise?
* How much inventory is below the reorder point?
* Which categories carry the highest inventory value?
* Where are forecast errors concentrated?
* Which suppliers have weaker on-time delivery performance?
* Which inventory areas require immediate attention?

This project addresses these questions through a combination of **Python-based data analysis and Power BI visualization**.

---

## 📊 Dataset

The dataset contains **1,000 SKU-level inventory records** with operational, financial, supplier, demand, and risk-related information.

### Main data areas

| Area      | Examples                                                |
| --------- | ------------------------------------------------------- |
| Product   | SKU, Category, ABC Class                                |
| Supplier  | Supplier ID, Supplier Name, On-Time Performance         |
| Warehouse | Warehouse ID, Location                                  |
| Inventory | Quantity on Hand, Reserved, Committed, Damaged, Returns |
| Demand    | Average Daily Sales, Forecast, Forecast Accuracy        |
| Financial | Unit Cost, Purchase Price, Inventory Value              |
| Risk      | Reorder Gap, Safety Stock Gap, ATP, Risk Score          |
| Dates     | Received Date, Purchase Date, Expiry Date, Audit Date   |

---

## 🐍 Python Analysis

Python was used as the main data preparation and analytical layer.

### Data Understanding

* Dataset structure and dimensions
* Data types
* Numerical and categorical variables
* Initial statistical exploration

### Data Quality

* Missing value analysis
* Data type validation
* Date validation
* Numeric consistency checks
* Business-rule validation

### Data Cleaning

* Standardized data types
* Validated date fields
* Checked numerical consistency
* Prepared the dataset for downstream analysis

### Business Validation

Pre-calculated business metrics were validated against their underlying operational variables.

Examples include:

* Available-to-Promise
* Inventory Value
* Forecast Error
* Reorder Gap
* Safety Stock Gap
* Stock Coverage
* Inventory Risk Score

This ensured that analytical features were consistent with the source inventory data.

---

## ⚙️ Feature Engineering

Several business-oriented analytical features were used to evaluate inventory health and operational risk.

Key features include:

* `Available_to_Promise`
* `Forecast_Error`
* `Forecast_Error_Pct`
* `Calculated_Inventory_Value`
* `Inventory_Value_Difference`
* `Inventory_Value_Diff_Pct`
* `Stock_Coverage_vs_LeadTime`
* `Reorder_Gap`
* `Safety_Stock_Gap`
* `Inventory_Risk_Score`
* `Supplier_Performance`

These features transform raw operational variables into metrics that are directly useful for supply chain decision-making.

---

## 📈 Key KPIs

The analysis focuses on several core inventory and supply chain KPIs:

* **Total Inventory Value**
* **Total SKUs**
* **Total Inventory Units**
* **Average Days of Inventory**
* **Negative ATP SKUs**
* **Reorder Risk %**
* **Safety Stock Risk %**
* **Forecast Accuracy**
* **Supplier On-Time Performance**
* **Inventory Risk Score**

---

## 🔎 Key Findings

The analysis identified several important inventory patterns:

* **1,000 SKUs** were analyzed.
* Total inventory value was approximately **$1.26M**.
* **28 SKUs** had negative Available-to-Promise.
* Approximately **25.6% of SKUs** were identified as being below the reorder point.
* Approximately **6.3% of SKUs** were below safety stock.
* Average supplier on-time performance was approximately **84.7%**.
* Average demand forecast accuracy was approximately **79.0%**.
* **Beverages** represented approximately **21.8% of total inventory value**.

These findings highlight areas where inventory availability, working capital, demand planning, and supplier performance can be improved.

---

## 📊 Power BI Dashboard

Power BI was used to transform the analytical dataset into a business-facing dashboard.

### Dashboard 1 — Executive Overview

The first dashboard provides a high-level view of inventory performance, including:

* Total Inventory Value
* Total SKUs
* Negative ATP
* Reorder Risk
* Forecast Accuracy
* Inventory Value by Category
* Inventory Risk by Category
* Inventory Status Distribution

### Dashboard 2 — Inventory Analysis

The second dashboard provides deeper analysis of:

* Inventory Value by ABC Class
* Supplier On-Time Performance
* Forecast Accuracy by Category
* Stock Coverage by Category

The dashboard is designed to communicate the most important supply chain insights quickly and clearly.

---

## 💡 Business Recommendations

Based on the analysis, several actions can be considered:

### 1. Prioritize Reorder-Risk SKUs

SKUs below their reorder point should be reviewed based on demand, lead time, and current available inventory.

### 2. Investigate Negative ATP

Negative ATP values indicate potential availability issues and should be investigated to prevent service-level problems.

### 3. Improve Safety Stock Planning

SKUs below safety stock should be evaluated against demand variability and supplier lead times.

### 4. Focus on High-Value Categories

Categories with a large share of inventory value should receive additional attention because inventory inefficiencies can have a greater financial impact.

### 5. Improve Supplier Performance

Suppliers with weaker on-time delivery performance may require performance reviews, lead-time reassessment, or corrective actions.

### 6. Improve Forecasting

Categories with lower forecast accuracy should be reviewed to identify demand variability and potential forecasting improvements.

---

## 🛠️ Tools & Technologies

* **Python**
* **Pandas**
* **NumPy**
* **Matplotlib**
* **Jupyter Notebook**
* **Power BI**
* **DAX**
* **Microsoft Excel**
* **GitHub**

---

## 📁 Project Structure

```text
Supply-Chain-Inventory-Analytics/
│
├── README.md
│
├── data/
│   └── supply_chain_inventory_clean.xlsx
│
├── notebooks/
│   └── supply_chain_inventory_analysis.ipynb
│
└── powerbi/
    └── supply_chain_inventory_dashboard.pbix
```

---

## 🔄 Analytical Workflow

```text
Raw Inventory Data
        ↓
Python Data Understanding
        ↓
Data Quality Assessment
        ↓
Data Cleaning
        ↓
Business Validation
        ↓
Feature Engineering
        ↓
KPI & Risk Analysis
        ↓
Clean Analytical Dataset
        ↓
Power BI Dashboard
        ↓
Business Insights & Recommendations
```

---

## 🎓 Project Objective

This project was developed as a portfolio project to demonstrate practical skills in:

* Data cleaning and validation
* Exploratory data analysis
* Feature engineering
* KPI development
* Supply chain analytics
* Inventory risk analysis
* Business intelligence
* Power BI dashboard development
* Data-driven business recommendations

The project demonstrates how raw operational data can be transformed into a structured analytical solution that supports supply chain decision-making.

