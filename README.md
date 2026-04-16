

# 📊 Superstore Profitability & Pricing Strategy Analysis

## 📌 Project Overview
This project performs an end-to-end **Exploratory Data Analysis (EDA)** and **Statistical Modeling** on a retail transaction dataset to identify the core drivers of profitability. The goal is to move beyond simple descriptive statistics and use **Multivariate Analysis** to provide actionable pricing recommendations.

### 🎯 Key Objectives
* Identify the "Profit Killers" within the product catalog.
* Quantify the statistical impact of **Discounts** on net margins.
* Isolate regional and segment-based performance anomalies.
* Provide a data-driven strategy for discount thresholds.

---

## 🛠️ Tech Stack
* **Language:** Python 3.x
* **Libraries:** * `Pandas` / `NumPy`: Data manipulation and type casting.
    * `Seaborn` / `Matplotlib`: Advanced multivariate visualization.
    * `Statsmodels`: OLS Linear Regression and statistical significance testing.

---

## 🔍 Analytical Approach

### 1. Data Engineering & Cleaning
* Handled categorical encoding using **One-Hot Encoding** (Dummy Variables) with `drop_first=True` to avoid the Dummy Variable Trap.
* Enforced strict numeric type casting for regression stability.
* Managed outliers to ensure robust statistical summaries.

### 2. Multivariate EDA
* **Interaction Analysis:** Used grouped boxplots to visualize the "Toxic Combination" of high discounts and specific categories (e.g., Furniture).
* **Pivot Heatmapping:** Created density maps of average profit margins across Regions and Segments to pinpoint operational drains.
* **Correlation Mapping:** Analyzed the relationship between Sales, Quantity, and Discounts.

### 3. Statistical Modeling (OLS)
Developed an **Ordinary Least Squares (OLS) Regression** model to isolate variables. 
* **Key Finding:** The model revealed that **Discounting** is the single largest predictor of negative profit ($p < 0.001$), with a coefficient of **-236.28**.

---

## 💡 Top Business Insights
* **The Discount Threshold:** For every 1% increase in discount, profit drops by approx. **$2.36**. Discounts over 20% in the Furniture category consistently lead to net losses.
* **Category Economics:** Technology and Office Supplies maintain superior margins compared to Furniture, even at similar sales volumes.
* **Regional Audit:** The **Central Region** is currently the primary drain on total profitability; an immediate pricing audit is recommended for this territory.

---

## 🚀 How to Run
1. Clone the repo:
   ```bash
   git clone https://github.com/soliana-k/Superstore-End-to-End-EDA.git
   ```
2. Install dependencies:
   ```bash
   pip install pandas numpy seaborn matplotlib statsmodels
   ```
3. Open the Jupyter Notebook:
   ```bash
   jupyter notebook superstory.ipynb
   ```

---

## 👨‍💻 Author
**Kalkidan Kassahun** *Master of Financial Engineering Candidate | Software Engineer* [https://www.linkedin.com/in/kalkidan-kassahun/]

---
