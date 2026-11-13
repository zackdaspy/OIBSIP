# Customer Segmentation Analysis (RFM & K-Means Clustering)

**Internship Track:** Data Analytics — Level 1, Task 2  
**Organization:** Oasis Infobyte (OIBSIP)

---

## Project Overview
This project segments an e-commerce customer base into distinct behavioral groups using **RFM (Recency, Frequency, Monetary)** analysis and **K-Means clustering**[cite: 30, 31]. By identifying high-value loyalists, growth-potential shoppers, and at-risk segments, the analysis provides targeted marketing recommendations to improve retention and customer lifetime value[cite: 30, 31].

---

## Tech Stack & Libraries
* **Language:** Python 3
* **Data Manipulation:** `pandas`, `numpy`
* **Machine Learning:** `scikit-learn` (`StandardScaler`, `KMeans`)
* **Data Visualization:** `matplotlib`, `seaborn`[cite: 31]
* **Environment:** Google Colab / Jupyter Notebook[cite: 31]

---

## Dataset Information
* **Source:** Kaggle — Online Retail / E-Commerce Dataset (`data.csv`)[cite: 31]
* **Key Features:** `InvoiceNo`, `StockCode`, `Description`, `Quantity`, `InvoiceDate`, `UnitPrice`, `CustomerID`, `Country`

---

## Analysis Workflow
1. **Data Cleaning:** Removed rows with missing `CustomerID` values, excluded cancelled invoices (`InvoiceNo` starting with `'C'`), and filtered out non-positive quantities and unit prices[cite: 31].
2. **RFM Feature Engineering:** Aggregated transaction records per customer to compute **Recency** (days since last purchase), **Frequency** (unique invoice count), and **Monetary** (total revenue generated)[cite: 31].
3. **Preprocessing & Scaling:** Applied log transformation (`np.log1p`) to handle skewed distributions, followed by `StandardScaler` standardization[cite: 31].
4. **Optimal Cluster Selection:** Used the **Elbow Method** across $K = 1$ to $10$ to determine **$K = 4$** as the optimal number of clusters[cite: 31].
5. **Clustering & Visualization:** Trained the K-Means model ($K = 4$), visualized cluster separations across RFM combinations using scatter plots, and plotted customer distribution per segment[cite: 31].

---

## Customer Segments & Marketing Recommendations
1. **Champions / VIP Loyalists:** Lowest recency, highest purchase frequency, and highest total spend. *Action:* Reward with VIP loyalty tiers, early access to new products, and referral incentives.
2. **Potential Loyalists:** Recent shoppers with moderate frequency and basket size. *Action:* Offer personalized cross-sell recommendations and free-shipping thresholds to increase order frequency.
3. **At-Risk Customers:** Previously active buyers who have not purchased recently. *Action:* Trigger automated win-back campaigns with time-limited discount vouchers.
4. **Hibernating / One-Time Buyers:** Highest recency and lowest frequency/spend. *Action:* Include in low-cost seasonal clearance promotions without heavy paid-ad spend.

---

## Repository Contents
* `Customer_Segmentation.ipynb` — Complete Jupyter Notebook with RFM preprocessing, K-Means clustering, visualizations, and marketing insights[cite: 2, 31].
* `README.md` — Project documentation and segment summary[cite: 2].
