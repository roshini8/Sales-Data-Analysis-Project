# 📊 Global Sales Data Analysis (2003–2005)

Gain deep insights into global sales performance across regions, product lines, and customer segments from 2003 to 2005 using Python-based data analysis and visualizations. This project focuses on data cleaning, transformation, and EDA to uncover patterns that can drive business decisions.

---

## 🎯 Project Goals

- 📈 Track yearly sales trends and growth
- 🛍️ Identify best-selling product lines and regions
- 💼 Analyze revenue by deal size and customer segments
- 🧹 Clean and preprocess raw data for analysis
- 📊 Build clear, compelling visualizations

---

## 📁 Dataset Overview

`global_sales.csv` contains **2,823 records** and **19 attributes**, covering orders, sales revenue, product details, customer demographics, and more.

| Column           | Description                           |
|------------------|---------------------------------------|
| `ORDERNUMBER`    | Unique identifier for each order      |
| `ORDERDATE`      | Date the order was placed             |
| `SALES`          | Total transaction revenue             |
| `PRODUCTLINE`    | Product category                      |
| `CUSTOMERNAME`   | Name of the customer                  |
| `COUNTRY`        | Country of the customer               |
| `DEALSIZE`       | Size of the deal (Small, Medium, Large) |
| `QUANTITYORDERED`| Quantity of items purchased           |
| `PRICEEACH`      | Unit price                            |

---

## 🧼 Data Preprocessing

- ✅ Converted `ORDERDATE` to datetime
- ✅ Created new columns: `Order_Year`, `Order_Month`, `Order_Weekday`
- ✅ Filled missing values in `STATE` and `POSTALCODE`
- ✅ Removed duplicate rows
- ✅ Checked for outliers in `PRICEEACH`

---

## 📊 Exploratory Analysis Highlights

- 🔥 **Heatmap**: Discovered strong correlations between quantity, price, and sales
- 🌍 **Top Regions**: Identified top-performing countries by total revenue
- 📅 **Revenue Trends**: Revealed consistent YoY growth (2003–2005)
- 🛍️ **Best Product Lines**: Pinpointed the most profitable product categories
- 💼 **Deal Size**: Found that Medium-sized deals dominate in revenue

---

## 🛠 Tech Stack

| Tool        | Purpose                    |
|-------------|----------------------------|
| `pandas`    | Data cleaning & manipulation |
| `numpy`     | Numeric operations          |
| `matplotlib` & `seaborn` | Visualizations |
| `Jupyter Notebook` | Interactive analysis |

---

## 📸 Sample Visualizations

> _(Generated with `seaborn` & `matplotlib`)_

- 📈 Line Plot: Year-over-Year Revenue
- 🌍 Bar Chart: Revenue by Country
- 🛍️ Pie Chart: Product Line Distribution
- 💸 Histogram: Price Distribution
- 🔗 Heatmap: Variable Correlations

---

## 🚀 How To Run

1. Clone the repo or download the `.ipynb` file
2. Open with **Jupyter Notebook** or **VS Code**
3. Load the dataset by updating the path:

```python
import pandas as pd
file_path = r"C:\path\to\global_sales.csv"
df = pd.read_csv(file_path)
```
