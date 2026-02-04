# Customer Shopping Behavior Analysis

## Project Overview
This project analyzes customer shopping behavior using transactional data from 3,900 purchases across multiple product categories. The objective is to derive actionable insights related to customer spending patterns, product preferences, discount usage, and subscription behavior to support data-driven business decisions.

The project implements a complete data analytics workflow including data cleaning, feature engineering, database integration, SQL-based analysis, and interactive dashboard visualization.

---

## Dataset Summary
- Total Records: 3,900
- Total Columns: 18

### Key Features
**Customer Demographics**
- Age
- Gender
- Location
- Subscription Status

**Purchase Information**
- Item Purchased
- Product Category
- Purchase Amount
- Season
- Size
- Color

**Behavioral Attributes**
- Discount Applied
- Promo Code Used
- Previous Purchases
- Purchase Frequency
- Review Rating
- Shipping Type

### Data Quality
- 37 missing values identified in the Review Rating column
- Missing values were imputed using the median rating for each product category

---

## Exploratory Data Analysis (Python)
Initial data exploration and preparation were conducted using Python and Pandas.

### Key Steps
- Loaded and inspected the dataset using `df.info()` and `df.describe()`
- Handled missing values in the Review Rating column
- Standardized column names using snake_case
- Feature engineering:
  - Created age_group by binning customer ages
  - Derived purchase_frequency_days
- Identified redundancy between discount_applied and promo_code_used and removed the redundant column
- Loaded the cleaned dataset into PostgreSQL for structured SQL analysis

---

## Data Analysis Using SQL (PostgreSQL)
SQL queries were used to answer business-driven analytical questions.

### Analysis Highlights
1. Revenue comparison by gender
2. Identification of high-spending customers using discounts
3. Top five products based on average review ratings
4. Comparison of average purchase value by shipping type
5. Spending analysis between subscribers and non-subscribers
6. Products with the highest dependency on discounts
7. Customer segmentation into new, returning, and loyal customers
8. Top three products within each category
9. Relationship between repeat purchases and subscription likelihood
10. Revenue contribution by age group

---

## Power BI Dashboard
An interactive Power BI dashboard was developed to visualize key metrics and trends, including revenue distribution, customer segments, product performance, subscription behavior, and discount impact. The dashboard enables stakeholders to quickly interpret insights and support strategic decision-making.

<img width="1172" height="638" alt="image" src="https://github.com/user-attachments/assets/300c6f80-d846-4c42-9b82-02bdbad392fe" />
---

## Business Recommendations
- Increase subscription adoption through exclusive subscriber benefits
- Implement loyalty programs to convert returning customers into loyal customers
- Optimize discount strategies to balance revenue growth and profitability
- Promote high-performing and highly rated products
- Focus marketing efforts on high-revenue age groups and premium shipping users

---

## Tools and Technologies
- Python (Pandas, NumPy)
- PostgreSQL
- SQL
- Power BI
- Jupyter Notebook / VS Code

---


## citation 
Amlan Mohanty from youtube 




