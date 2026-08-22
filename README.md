# Task 13 — Restaurant Branch Performance EDA

## Project Overview

This project performs Exploratory Data Analysis (EDA) on a restaurant branch performance dataset using **Pandas, NumPy, and Matplotlib**.

The analysis follows the Day 13 EDA concepts from the provided notes: understanding the dataset, descriptive statistics, univariate analysis, categorical analysis, distribution analysis, grouped/bivariate analysis, and correlation analysis. The notes specifically frame EDA as a way to understand patterns and relationships between variables, with examples using `shape`, `dtypes`, `describe()`, `value_counts()`, grouped analysis, and correlation. fileciteturn0file0L22-L31

## Dataset

- **Rows:** 350
- **Columns:** 22
- **Time period:** January–June 2026
- **Main business variables:** Customers, Orders, Average Bill, Revenue, Food Cost, Operating Cost, Profit, Marketing Spend, Staff Count, Average Delivery Time, Customer Rating
- **Categorical dimensions:** Branch, Region, Store Type, Day, Month, Weather, Promotion

## Repository Structure

```text
Task 13/
├── Restaurant_Branch_Performance.ipynb
├── Day13_Restaurant_Branch_Performance_Dataset.csv
├── README.md
└── requirements.txt
```

## What the Notebook Covers

1. Dataset loading and structure
2. Shape, data types, and basic inspection
3. Missing-value and duplicate checks
4. Numerical summary statistics
5. Categorical frequency analysis
6. Distribution analysis using histograms
7. IQR-based outlier inspection and boxplots
8. Branch performance comparison
9. Region performance comparison
10. Store type comparison
11. Day and month analysis
12. Marketing, staffing, delivery, rating, and promotion analysis
13. Numerical correlation matrix
14. Focused relationship/scatter-plot analysis
15. 8 final data-driven observations

## Key Findings

- **Customers vs Orders:** correlation ≈ **0.98**, showing an extremely strong positive relationship.
- **Revenue vs Profit:** correlation ≈ **0.97**, indicating that higher revenue is strongly associated with higher profit.
- **Premium stores** have the highest average revenue and profit, while Express stores have substantially lower average values.
- **South** has the highest average revenue and profit among the three regions.
- **Bengaluru** has the highest average branch profit, while **Mumbai** has the lowest.
- **Marketing Spend vs Revenue:** correlation ≈ **0.43**, a moderate positive relationship.
- **Delivery Time vs Customer Rating:** correlation ≈ **-0.44**, a moderate negative relationship.
- Revenue, Food Cost, Operating Cost, and Profit show positive skewness, with several IQR-based high-end outliers.

## Important Interpretation Note

Correlation identifies linear association; it does **not** prove causation. Group comparisons should also be interpreted with record counts in mind, especially for store types and branches.

## How to Run

### Jupyter Notebook

```bash
pip install -r requirements.txt
jupyter notebook Restaurant_Branch_Performance.ipynb
```

### Google Colab

Upload the notebook and CSV together, then run the notebook cells from top to bottom. If the CSV is uploaded to the Colab working directory, the existing file path will work directly.

## Tools Used

- Python
- Pandas
- NumPy
- Matplotlib
- Jupyter Notebook / Google Colab
