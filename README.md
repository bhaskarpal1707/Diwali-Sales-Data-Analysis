
# 🛍️ Diwali Sales Data Analysis

## 📌 Subtitle
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

This EDA solves several real-world business questions:

- ✅ Who are the most profitable customer demographics?
- 📍 Which zones and states drive the most revenue?
- 🛒 What are the top-performing product categories?
- 💰 How does purchase behavior affect revenue?
- ⚠️ Which regions or customer segments need improvement?

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

```python
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns

df = pd.read_csv("Sales.csv")

df.head()
df.info()
df.describe(include='all')
```

---

### 2️⃣ Data Cleaning

```python
df.drop(columns=["Status", "unnamed1"], inplace=True)
df.dropna(subset=["Amount"], inplace=True)
df['Marital_Status'] = df['Marital_Status'].astype(int)
df['Amount'] = df['Amount'].astype(float)
```

---

### 3️⃣ Exploratory Data Analysis (EDA)

#### Demographics and Behavior

```python
df['Gender'].value_counts()
df.groupby("Age Group")["Orders"].sum().sort_values(ascending=False)
```

#### Regional Analysis

```python
df.groupby("Zone")["Amount"].sum().sort_values(ascending=False)
df.groupby("State")["Orders"].sum().sort_values(ascending=False)
```

#### Product Analysis

```python
df.groupby("Product_Category")["Amount"].sum().sort_values(ascending=False)
df['Product_ID'].value_counts().head(10)
```

#### Visualizations

```python
sns.set(style="whitegrid")
df.groupby("Zone")["Amount"].sum().sort_values().plot(kind="bar", figsize=(8,5), color="skyblue", title="Sales by Zone")
plt.ylabel("Sales Amount")
plt.show()
```

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
