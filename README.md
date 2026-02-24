# Customer Shopping Analysis

An end-to-end Data Analytics project using Python, SQL, and Power BI to analyze customer shopping behavior and generate actionable business insights.

---

## Project Overview

This project focuses on analyzing customer purchase data to:

- Understand customer buying patterns  
- Identify top-performing product categories  
- Analyze revenue trends  
- Perform SQL-based business queries  
- Build an interactive Power BI dashboard  

---

## Project Structure

```
Customer-Shopping-Analysis/
│
├── Customer_Shopping_Analysis.ipynb
├── customer_analysis.sql
├── customer_analysis.csv
├── customer_analysis_dashboard.pbix
└── README.md
```

---

## Python Analysis

File: `Customer_Shopping_Analysis.ipynb`

Tasks performed:

- Data cleaning and preprocessing  
- Handling missing values  
- Exploratory Data Analysis (EDA)  
- Revenue and category analysis  
- Data visualization  

Libraries used:

- pandas  
- numpy  
- matplotlib  
- seaborn  

Example:

```python
import pandas as pd

df = pd.read_csv("customer_analysis.csv")

# Total Revenue
total_revenue = df["Total_Amount"].sum()

# Category-wise Sales
category_sales = df.groupby("Category")["Total_Amount"].sum()
```

---

## SQL Analysis (PostgreSQL)

File: `customer_analysis.sql`

Business queries performed:

- Total revenue calculation  
- Category-wise sales analysis  
- Monthly sales trends  
- Customer purchase frequency  
- Average order value  

Example:

```sql
SELECT category, SUM(total_amount) AS total_sales
FROM customer_analysis
GROUP BY category
ORDER BY total_sales DESC;
```

---

## Power BI Dashboard

File: `customer_analysis_dashboard.pbix`

Dashboard includes:

- Total Revenue KPI  
- Monthly Sales Trends  
- Category-wise Performance  
- Customer Insights  
- Interactive Filters  

The dashboard provides dynamic and interactive visualization of business metrics.

---

## Project Workflow

1. Data collection (CSV file)  
2. Data cleaning and EDA using Python  
3. Data import into PostgreSQL  
4. SQL business queries  
5. Dashboard creation in Power BI  

---

## Key Insights

- Identified top-performing product categories  
- Analyzed customer spending distribution  
- Evaluated monthly revenue patterns  
- Highlighted valuable customer segments  

---

## Tools and Technologies

- Python  
- PostgreSQL  
- Power BI  
- Jupyter Notebook  

---

## How to Run

### Python
Open the Jupyter Notebook and run all cells.

### SQL
Import the dataset into PostgreSQL and execute queries from `customer_analysis.sql`.

### Power BI
Open the `.pbix` file in Power BI Desktop and refresh data if needed.

---

## Author

Rakshith S  
Data Analytics Enthusiast  
Python | SQL | Power BI
