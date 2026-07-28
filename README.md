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

<img src="https://github.com/user-attachments/assets/c8fa40d3-7c31-44c9-abab-d7716ba7b469" width="600" />
<br><br>
<img src="https://github.com/user-attachments/assets/d5b98ebf-d108-44dc-962a-c2ec58ce6aea" width="600" />

> **🔍 Analytical Insights:**
> * **Left-Skewed Distribution:** Both `Qty Sold` and `Turnover Index` exhibit pronounced left-skewness, driven by negative transaction values representing customer product returns.
> * **High Sales Volatility:** A high standard deviation ($\sigma = \$75.11$) in `Sales Amount` highlights significant daily sales fluctuation linked to promotional order spikes.
> * **Business Impact:** Unfiltered negative return transactions distort revenue forecasting and obscure true baseline sales performance.
---

### 2. Store Stockout Risk vs. Inventory Buffer

<img src="https://github.com/user-attachments/assets/298b0231-2068-4178-848b-474f68eccba3" width="700" />

> **🔍 Analytical Insights:**
> * **Critical Buffer Vulnerability:** Store-level inventory distribution indicates a `Qty on Hand` mode of just **1 unit**, exposing retail outlets to severe stockout risks during peak demand periods.
> * **Inventory Imbalance:** High-velocity outlets consistently face stock shortage risks, while lower-turnover locations hold excessive deadstock.
> * **Business Impact:** Misaligned stock allocation leads to lost sales opportunities, reduced customer satisfaction, and inflated holding costs in low-performing stores.
---

### 3. Profitability Erosion due to Product Returns

<img src="https://github.com/user-attachments/assets/bb0cde34-f01a-4f27-ab37-9c3d8aadc0f3" width="700" />

> **🔍 Analytical Insights:**
> * **Margin Degradation:** Unmanaged reverse logistics and product return processing costs directly erode gross margins across top-performing sales channels.
> * **Category Concentration:** Negative margin trends are disproportionately driven by specific product categories experiencing high return volumes.
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

```
---
## 🤝 Connect & Feedback

| Attribute | Details |
| :--- | :--- |
| **Developer** | **Agalya J.** |
| **Role** |Data Analyst |
| **Project Repo** | [Inventory-Optimization-Analysis](https://github.com/agalya-data-analyst/Inventory-Optimization-Analysis) |
| **LinkedIn Profile** | [Connect on LinkedIn](https://www.linkedin.com/in/agalyajayapal/) |

---
