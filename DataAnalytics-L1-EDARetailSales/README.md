# Exploratory Data Analysis (EDA) on Retail Sales Data

**Internship Track:** Data Analytics — Level 1, Task 1  
**Organization:** Oasis Infobyte (OIBSIP)

---

## Project Overview
This project performs a comprehensive Exploratory Data Analysis (EDA) on a retail sales dataset to uncover purchasing patterns, seasonal sales trends, customer demographics, and top-performing product categories. The insights derived from this analysis are translated into actionable business recommendations to support data-driven decision-making.

---

## Tech Stack & Libraries
* **Language:** Python 3
* **Data Manipulation:** `pandas`, `numpy`
* **Data Visualization:** `matplotlib`, `seaborn`
* **Environment:** Jupyter Notebook / Google Colab

---

## Dataset Information
* **Source:** Kaggle (`retail_sales_dataset.csv`)
* **Key Features:** `Transaction ID`, `Date`, `Customer ID`, `Gender`, `Age`, `Product Category`, `Quantity`, `Price per Unit`, `Total Amount`

---

## Analysis Workflow
1. **Data Loading & Inspection:** Checked dataset dimensions, column data types, duplicate entries, and missing values.
2. **Descriptive Statistics:** Computed mean, median, mode, and standard deviation across numerical attributes.
3. **Time Series Analysis:** Analyzed monthly and quarterly revenue trends to identify peak periods and seasonal dips.
4. **Customer Demographics:** Examined age distributions and gender breakdowns across transactions.
5. **Product Performance:** Evaluated revenue contribution by product category and identified top-performing products/orders.
6. **Correlation Analysis:** Generated a correlation heatmap to measure relationships between numerical variables (`Age`, `Quantity`, `Price per Unit`, `Total Amount`).
7. **Category & Demographic Spending:** Compared order value distributions across product categories segmented by gender.

---

## Key Findings
*(Replace the placeholders below with your actual numbers after running the notebook)*
* **Sales Trends:** Peak sales occurred in `[Insert Peak Month/Quarter]`, while `[Insert Lowest Month/Quarter]` recorded the lowest revenue.
* **Customer Profile:** The core customer base falls within the `[Insert Age Range, e.g., 25–45]` age group, with a `[Insert Male % / Female %]` gender split.
* **Top Categories:** `[Insert Top Category]` generated the highest overall revenue, followed by `[Insert Second Category]`.
* **Correlation:** `Total Amount` shows a strong positive correlation with `Price per Unit` and `Quantity`, whereas `Age` shows minimal linear correlation with order value.

---

## Business Recommendations
1. **Seasonal Inventory & Promotions:** Increase inventory allocation ahead of `[Insert Peak Quarter]` and introduce targeted discount campaigns during `[Insert Low Month]` to stabilize off-peak revenue.
2. **Demographic-Focused Marketing:** Tailor digital ad campaigns and loyalty rewards toward the `[Insert Dominant Age Bracket]` demographic, focusing on high-performing categories like `[Insert Top Category]`.
3. **Cross-Selling & Bundling:** Bundle lower-priced items with high-demand products in `[Insert Top Category]` to increase average units per transaction (`Quantity`).

---

## Repository Contents
* `EDA_Retail_Sales.ipynb` — Complete Jupyter Notebook with code, visualizations, and markdown observations.
* `retail_sales_dataset.csv` — Raw dataset used for the analysis.
* `README.md` — Project documentation and summary of findings.
