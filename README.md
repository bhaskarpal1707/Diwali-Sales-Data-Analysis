# 🛍️ Diwali Sales Data Analysis

**Uncovering Customer Trends, Product Demand & Regional Performance from Diwali Sales Data**

---

## 📋 Objective

The objective of this analysis is to perform a detailed **Exploratory Data Analysis (EDA)** on Diwali sales data collected across India. This analysis uncovers hidden patterns, trends, and actionable business insights to support strategic decisions in:

- Customer segmentation
- Marketing strategy optimization
- Product demand forecasting
- Regional targeting

---

## 🧩 Business Problems Addressed

Through Exploratory Data Analysis, the following business problems are addressed:

- • Identify the most profitable customer demographics (age, gender, marital status, occupation).
- • Understand regional sales performance to improve localized promotions.
- • Determine top-selling product categories and associated sales volumes.
- • Evaluate the impact of customer behavior (orders, purchase amount) on revenue.
- • Discover underperforming segments for targeted improvement.

---

## 🛠️ Tools & Technologies Used

- **Python**: Core language
- **Pandas**: Data manipulation
- **Matplotlib & Seaborn**: Data visualization
- **Jupyter Notebook**: Interactive development

---

## 🗂️ Dataset Overview

- 📄 Filename: `Sales.csv`
- 📈 Records: 11,251 rows
- 🔢 Key Features:
  - `User_ID`, `Cust_name`
  - `Gender`, `Age`, `Marital_Status`, `Occupation`
  - `State`, `Zone`
  - `Product_Category`, `Orders`, `Amount`

---

## 🔄 Project Workflow

### 1️⃣ Data Load & Inspection

- Load the sales dataset into a Pandas DataFrame.
- Display the first few rows to understand the data structure.
- Check the data types and non-null values for each column to identify initial data quality issues.
- View descriptive statistics to understand the distribution of numerical data.

```

---

### 2️⃣ Data Cleaning

- Dropping Unnecessary Columns: Remove irrelevant columns that do not contribute to the analysis (e.g., unnamed1).
- Handling Missing Values: Identify and handle (e.g., drop) rows with missing values to ensure data integrity for analysis.
- Correcting Data Types: Convert columns to appropriate data types if necessary (e.g., Marital_Status to integer, Amount to float).

---

### 3️⃣ Exploratory Data Analysis (EDA)

- Gender Distribution & Gender-wise Total Sales: Analyze the number of buyers and total sales amount for each gender.
- Age Group Distribution & Age Group-wise Total Sales: Examine the distribution of sales across different age groups and their total sales contributions.
- State-wise Total Orders & Sales: Identify the top-performing states based on the number of orders and total sales amount.
- Marital Status & Sales: Analyze the total sales amount based on the marital status of the customers.
- Occupation & Sales: Visualize and understand the total sales amount across various occupations.
- Product Category & Sales: Determine the top-selling product categories by total sales amount.
- Top 10 Most Sold Products: Identify and display the top 10 products based on the number of orders.
- Orders vs Amount Scatter Plot: Visualize the relationship between the number of orders and the total amount spent.
- Top 10 Customers by Sales: Identify and analyze the highest-spending customers.
- Average Order Value by State (Top 10): Calculate and visualize the average amount spent per order in the top states.
- Age Distribution Histogram: Visualize the distribution of customer ages.
- Repeat Customers Count Distribution: Analyze the frequency of purchases by customers.
- Correlation Heatmap (Age, Orders, Amount): Visualize the correlation between numerical variables to understand their relationships.

---

## 💡 Key Insights

- 🎯 Female customers aged 26–35 are the most profitable segment.
- 🥇 Central and Southern zones are top-performing.
- 🛒 Food, Clothing & Electronics dominate product sales.
- ⚖️ Orders correlate strongly with amount spent.
- 📉 Certain regions and occupations underperform.

---

## 🧾 Business Outcomes

- Clear target audience for focused marketing.
- Better product stocking and planning.
- Insightful regional expansion strategies.
- Reliable base for predictive modeling.

---

## 📈 Visual Summary

| Insight         | Description                       |
|----------------|-----------------------------------|
| Central Zone   | ₹41.6M in sales                   |
| Top Product    | Food – ₹33.9M                     |
| Leading Age    | 26–35 year-olds                   |
| Gender Dominant| ~70% Female                       |
| Power Buyers   | Repeat customers identified       |

---

## 📚 Future Scope

- Time-series forecasting
- Customer segmentation clustering
- Campaign optimization by region and gender
- Churn prediction modeling

---

## 🏁 Conclusion

This project uses EDA to derive actionable insights from Diwali sales data. It supports smarter decision-making across product, customer, and regional strategies.

---

## 📂 Repository Structure

```
📁 Diwali-Sales-Analysis/
├── Sales.csv
├── Sales Analysis.ipynb
├── README.md
└── Visuals/
```

---
## 📬 Contact

For queries or collaborations:
**Bhaskar Pal**
📧 [bhaskarpal.official@gmail.com](mailto:bhaskarpal.official@gmail.com)

---

## 📜 License

Licensed under the MIT License.
