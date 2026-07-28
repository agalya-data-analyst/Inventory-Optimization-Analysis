# 📦 Multi-Channel Supply Chain Warehouse Inventory & Safety Stock Optimization

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/agalya-data-analyst/Inventory-Optimization-Analysis/blob/main/notebooks/Supplychain_Inventory.ipynb)
![Python](https://img.shields.io/badge/Python-3.10%2B-blue)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458)
![Status](https://img.shields.io/badge/Project-Completed-success)

---

## 📌 Executive Summary

This project delivers an end-to-end data analytics framework designed to analyze multi-channel retail inventory, reduce stockout vulnerabilities, and optimize warehouse dynamic safety stock buffers. By processing transaction-level order flows and store stock levels, the analytical model highlights stock imbalance bottlenecks and financial leakage driven by unmanaged customer returns.

---

## 🎯 Key Business Objectives

* **Sales Volatility & Demand Analysis:** Evaluate monthly sales trends, promotional price lifts, and category-level demand distribution across store networks.
* **Stockout & Deadstock Identification:** Cross-analyze `Qty Sold` against store `Qty on Hand` to flag critical retail inventory vulnerabilities.
* **Return-Induced Profit Erosion:** Quantify net revenue losses caused by negative sales transaction returns ($<0$).
* **Dynamic Safety Stock Modeling:** Establish responsive buffer thresholds to prevent stockouts while minimizing deadstock holding costs.

---

## 🛠️ Tech Stack & Analytical Libraries

* **Core Language:** Python 3.10+
* **Environment:** Google Colab
* **Data Manipulation & Processing:** Pandas, NumPy
* **Data Visualization:** Matplotlib, Seaborn
* **Version Control & Repository:** GitHub
* **Documentation & Reporting:** Microsoft Word, PDF Formatting, Markdown (`.md`)

---

## 📊 Summary of EDA Findings & Key Metrics

| Analytical Category | Metric / Indicator | Key Statistical Finding | Strategic Business Impact |
| :--- | :--- | :--- | :--- |
| **Sales Distribution** | `Qty Sold` Mean | $0.94$ (Median: $1.00$) | Left-skewed due to customer return values ($<0$). |
| **Revenue Volatility** | `Sales Amount` Std Dev | $\sigma = \$75.11$ | High daily variance linked to promotional order spikes. |
| **Store Inventory Risk** | `Qty on Hand` Mode | $1.00$ Unit | Extreme stockout vulnerability during peak demand hours. |
| **Turnover Performance** | `Turnover Index` Mean | $-2.97$ | Profit erosion driven by unmanaged reverse logistics/returns. |

---

## 📈 Exploratory Data Analysis & Key Visualizations

### 1. Metric Distribution & Central Tendencies
> **Finding:** The distribution of `Qty Sold` and `Turnover Index` exhibits left-skewness driven by negative transaction values representing customer product returns.

<!-- INSERT YOUR HISTOGRAM / DISTRIBUTION CHART SCREENSHOT HERE -->
![Central Tendency & Metric Distribution](<img width="613" height="393" alt="image" src="https://github.com/user-attachments/assets/c8fa40d3-7c31-44c9-abab-d7716ba7b469" />
<img width="613" height="408" alt="image" src="https://github.com/user-attachments/assets/d5b98ebf-d108-44dc-962a-c2ec58ce6aea" />

)

---

### 2. Store Stockout Risk vs. Inventory Buffer
> **Finding:** Cross-analyzing store inventory reveals acute stockout vulnerabilities in high-velocity stores holding minimal stock ($1.00$ unit), while low-turnover stores hold excessive deadstock.

<!-- INSERT YOUR STORE COMPARISON / BAR CHART SCREENSHOT HERE -->
![Store Stockout Risk Analysis](<img width="1490" height="690" alt="image" src="https://github.com/user-attachments/assets/298b0231-2068-4178-848b-474f68eccba3" />
)

---

### 3. Profitability Erosion due to Product Returns
> **Finding:** Unmanaged product returns directly erode gross sales margins, driving net profit performance down across impacted product categories.

<!-- INSERT YOUR PROFIT EROSION / RETURN LOSS CHART SCREENSHOT HERE -->
![Profitability & Return Rate Mitigation](<img width="689" height="474" alt="image" src="https://github.com/user-attachments/assets/bb0cde34-f01a-4f27-ab37-9c3d8aadc0f3" />
)

---

## 💡 Strategic Business Recommendations

1. **Dynamic Safety Stock Policy:** Transition from flat-rate inventory rules to dynamic buffer thresholds—holding $1\text{--}3$ units for low-velocity SKUs and scaling up to $20$ units for high-demand items to minimize holding costs.
2. **Inter-Store Inventory Transfers:** Reallocate surplus stock from low-turnover stores to high-demand locations experiencing stockout vulnerabilities.
3. **Return Rate Mitigation:** Address root causes of customer returns (such as sizing accuracy and quality control) to prevent negative sales quantities from eroding profit margins.

---

## 📂 Repository Structure

```text
Inventory-Optimization-Analysis/
│
├── data/
│   └── Raw_Sales_and_Inventory_Data.xlsx     # Primary Multi-channel Dataset
│
├── notebooks/
│   └── Supplychain_Inventory.ipynb           # Complete Colab Analysis Code
│
├── Documentation/
│   └── Final_Project_Report.pdf              # Comprehensive PDF Documentation Report
│
└── README.md                                 # Main Project Documentation

## 👤 ## 🤝 Connect & Feedback

| Attribute | Details |
| :--- | :--- |
| **Developer** | **Agalya J.** |
| **Role** |Data Analyst |
| **Project Repo** | [Inventory-Optimization-Analysis](https://github.com/agalya-data-analyst/Inventory-Optimization-Analysis) |
| **LinkedIn Profile** | [Connect on LinkedIn](https://www.linkedin.com/in/agalyajayapal/) |

---
