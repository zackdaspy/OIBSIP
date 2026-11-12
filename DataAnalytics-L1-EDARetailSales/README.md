# Exploratory Data Analysis (EDA) on Retail Sales Data

**Internship Track:** Data Analytics — Level 1, Task 1  
**Organization:** Oasis Infobyte (OIBSIP)

---

## Project Overview
This project performs a comprehensive Exploratory Data Analysis (EDA) on a retail sales dataset to uncover purchasing patterns, seasonal sales trends, customer demographics, and top-performing product categories. The insights derived from this analysis are translated into actionable business recommendations to support data-driven decision-making[cite: 30].

---

## Tech Stack & Libraries
* **Language:** Python 3
* **Data Manipulation:** `pandas`, `numpy`
* **Data Visualization:** `matplotlib`, `seaborn`[cite: 30]
* **Environment:** Jupyter Notebook / Google Colab[cite: 30]

---

## Dataset Information
* **Source:** Kaggle (`retail_sales_dataset.csv`)[cite: 30, 54]
* **Key Features:** `Transaction ID`, `Date`, `Customer ID`, `Gender`, `Age`, `Product Category`, `Quantity`, `Price per Unit`, `Total Amount`

---

## Analysis Workflow
1. **Data Loading & Inspection:** Checked dataset dimensions (1,000 rows, 9 columns), column data types, duplicate entries, and missing values[cite: 30].
2. **Descriptive Statistics:** Computed mean, median, mode, and standard deviation across numerical attributes[cite: 30].
3. **Time Series Analysis:** Analyzed monthly and quarterly revenue trends to identify peak periods and seasonal dips[cite: 30].
4. **Customer Demographics:** Examined age distributions and gender breakdowns across transactions[cite: 30].
5. **Product Performance:** Evaluated revenue contribution by product category and identified top-performing orders[cite: 30].
6. **Correlation Analysis:** Generated a correlation heatmap to measure relationships between numerical variables (`Age`, `Quantity`, `Price per Unit`, `Total Amount`)[cite: 30].
7. **Category & Demographic Spending:** Compared order value distributions across product categories segmented by gender[cite: 30].

---

## Key Findings
* **Sales Trends:** Peak sales occurred in **May and October** (Q2 and Q4), while **March and September** recorded the lowest revenue[cite: 54].
* **Customer Profile:** Customers span ages **18–64**, with a balanced gender split of **~51% Female and ~49% Male**[cite: 54].
* **Top Categories:** **Electronics** generated the highest overall revenue, closely followed by **Clothing** and **Beauty**[cite: 54].
* **Correlation:** `Total Amount` shows a strong positive correlation with `Price per Unit` (0.85) and `Quantity` (0.37), whereas `Age` shows minimal linear correlation (-0.06) with order value.

---

## Business Recommendations
1. **Seasonal Inventory & Promotions:** Increase inventory allocation ahead of **Q2 and Q4** and introduce targeted discount campaigns during **March and September** to stabilize off-peak revenue[cite: 54].
2. **Demographic-Focused Marketing:** Tailor digital ad campaigns and loyalty rewards across adult age brackets (**18–64**), focusing on high-performing categories like **Electronics** and **Clothing**[cite: 54].
3. **Cross-Selling & Bundling:** Bundle lower-priced items with high-demand products in **Electronics** to increase average units per transaction (`Quantity`)[cite: 54].

---

## Repository Contents
* `EDA_Retail_Sales.ipynb` — Complete Jupyter Notebook with code, visualizations, and markdown observations[cite: 54].
* `retail_sales_dataset.csv` — Raw dataset used for the analysis[cite: 54].
* `README.md` — Project documentation and summary of findings[cite: 54].
