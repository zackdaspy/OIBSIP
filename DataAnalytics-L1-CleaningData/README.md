# Data Cleaning & Preprocessing Pipeline

**Internship Track:** Data Analytics — Level 1, Task 3  
**Organization:** Oasis Infobyte (OIBSIP)

---

## Project Overview
This project demonstrates a systematic, end-to-end data cleaning workflow on the messy Titanic passenger dataset (`891 rows × 15 columns`), transforming raw, inconsistent records into an analysis-ready dataset with full documentation of every preprocessing decision[cite: 31, 32].

---

## Tech Stack & Libraries
* **Language:** Python 3
* **Data Manipulation:** `pandas`, `numpy`[cite: 31]
* **Dataset Source:** `seaborn` (`titanic` dataset)[cite: 32]
* **Environment:** Google Colab / Jupyter Notebook[cite: 31]

---

## Data Cleaning Workflow
1. **Initial Data Quality Report:** Audited null value counts/percentages per column, duplicate rows (`107`), inconsistent string formatting, and value range anomalies[cite: 31].
2. **Duplicate Removal:** Removed **107 exact duplicate rows** to eliminate statistical bias[cite: 31].
3. **Missing Data Handling:**
   * Dropped `deck` (**77.2%** missing) and redundant `alive` columns[cite: 31].
   * Imputed `age` (`177` missing) using the **median** (`28.0`) to resist skewness[cite: 31].
   * Imputed `embarked` and `embark_town` (`2` missing) using the **mode** (`S` / `Southampton`)[cite: 31].
4. **Standardization:** Normalized lowercase text strings in `sex`, `who`, and `embark_town` to uniform Title Case[cite: 31].
5. **Outlier Detection & Capping:** Applied the Interquartile Range ($1.5 \times \text{IQR}$) method to `fare`, capping upper-end outliers at **73.44**[cite: 31].
6. **Data Type Verification:** Converted categorical `pclass` identifiers to string (`object`) and standardized `fare` monetary values to 2-decimal `float`[cite: 31].

---

## Before vs. After Summary
| Metric | Before Cleaning | After Cleaning |
| :--- | :--- | :--- |
| **Total Rows** | 891 | 784 |
| **Total Columns** | 15 | 13 |
| **Total Missing (Null) Cells** | 869 | 0 |
| **Duplicate Rows** | 107 | 0 |

---

## Repository Contents
* `Data_Cleaning.ipynb` — Complete Jupyter Notebook with data quality audit, cleaning pipeline, and documented justifications[cite: 2, 31].
* `raw_titanic_dataset.csv` — Original raw dataset before preprocessing.
* `cleaned_titanic_dataset.csv` — Final cleaned, analysis-ready dataset exported to CSV[cite: 32].
* `README.md` — Project documentation and summary table.
