# Restaurant Branch Performance — Exploratory Data Analysis

## Project Overview

This project performs an Exploratory Data Analysis (EDA) of a restaurant branch performance dataset using **Python, Pandas, NumPy, and Matplotlib**.

The analysis focuses on understanding business performance, identifying patterns across branches and regions, examining operational factors, and exploring relationships between key numerical variables.

## Dataset

The dataset contains restaurant performance records with information about:

* Date, day, and month
* Branch and region
* Store type
* Staff count
* Marketing spend
* Customers and orders
* Average bill
* Revenue
* Food cost
* Operating cost
* Profit
* Average delivery time
* Customer rating
* Weather conditions
* Promotion information

## Analysis Performed

The notebook covers the following areas:

### 1. Dataset Overview

* Loaded the restaurant performance dataset using Pandas
* Examined dataset shape and structure
* Reviewed column data types
* Displayed sample records
* Checked for missing values
* Checked for duplicate records

### 2. Descriptive Statistics

* Calculated summary statistics for numerical variables
* Examined mean, median, standard deviation, quartiles, minimum, and maximum values
* Calculated skewness to understand the distribution of numerical variables

### 3. Categorical Analysis

Analyzed the distribution of categorical variables including:

* Branch
* Region
* Store Type
* Day
* Month
* Weather
* Promotion

Frequency counts were used to understand the representation of different categories in the dataset.

### 4. Distribution Analysis

Analyzed the distributions of key business variables using histograms and boxplots, including:

* Customers
* Revenue
* Profit
* Marketing Spend
* Staff Count
* Average Delivery Time
* Customer Rating

### 5. Outlier Analysis

Used the **Interquartile Range (IQR)** method to identify potential outliers in numerical variables.

Potential outliers were inspected rather than automatically removed, since unusually high or low values may represent genuine differences in restaurant performance.

### 6. Branch Performance Analysis

Compared branches based on:

* Average customers
* Average revenue
* Average profit
* Marketing spend
* Staff count
* Delivery time
* Customer ratings

### 7. Regional Analysis

Compared restaurant performance across regions to identify differences in:

* Customer volume
* Revenue
* Profit
* Marketing spend
* Staffing
* Delivery time
* Customer ratings

### 8. Store Type Analysis

Compared performance across different store types using average:

* Customers
* Revenue
* Profit
* Marketing spend
* Staff count
* Delivery time
* Customer ratings

### 9. Time-Based Analysis

Examined performance across days and months to identify variations in:

* Customer volume
* Revenue
* Profit
* Delivery time
* Customer ratings

### 10. Operational Analysis

Investigated relationships involving:

* Marketing spend
* Staff count
* Customers
* Revenue
* Profit
* Delivery time
* Customer ratings
* Promotion categories

### 11. Correlation Analysis

Created a correlation matrix for the numerical variables to identify the strength and direction of linear relationships.

Focused relationship plots were also used to examine important associations such as:

* Customers vs Revenue
* Marketing Spend vs Revenue
* Staff Count vs Customers
* Delivery Time vs Customer Rating
* Average Bill vs Profit

> **Note:** Correlation indicates association between numerical variables and does not establish causation.

## Key Findings

1. **Customers and Orders have an extremely strong positive relationship**, indicating that higher customer volume is closely associated with higher order volume.

2. **Revenue and Profit have a very strong positive relationship**, showing that higher revenue generally corresponds to higher profit in the dataset.

3. **Store type has a noticeable effect on average financial performance**, with Premium stores showing the highest average revenue and profit among the store categories.

4. **Performance varies across regions and branches**, with differences in average revenue, profit, customer volume, delivery time, and ratings.

5. **Marketing spend has a positive relationship with revenue**, although the relationship with profit is weaker, suggesting that higher marketing expenditure does not necessarily translate into a proportionally higher profit.

6. **Delivery time has a negative relationship with customer ratings**, indicating that observations with longer delivery times tend to have lower ratings.

7. **Revenue, Food Cost, Operating Cost, and Profit show positive skewness**, with some observations substantially higher than the typical values.

8. **The correlation analysis highlights customer volume, order volume, revenue, average bill, and profit as closely connected business variables**, providing useful insight into the main drivers of restaurant performance.

## Repository Structure

```text
Task 13/
├── Restaurant_Branch_Performance.ipynb
├── Day13_Restaurant_Branch_Performance_Dataset.csv
└── README.md
```

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Jupyter Notebook / Google Colab

## How to Run

1. Download or clone this repository.
2. Open `Restaurant_Branch_Performance.ipynb` in Jupyter Notebook, JupyterLab, or Google Colab.
3. Keep the CSV file in the same working directory as the notebook.
4. Run the notebook cells from top to bottom.

The notebook contains the complete EDA, including analysis tables, visualizations, correlation analysis, and final observations.
