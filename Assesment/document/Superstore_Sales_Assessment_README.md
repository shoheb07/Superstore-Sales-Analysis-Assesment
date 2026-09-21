# Superstore Sales Assessment Project

## 📊 Project Overview

The **Superstore Sales Assessment Project** is a practical Data Analytics project focused on assessing, cleaning, exploring, and interpreting retail sales data.

The project uses a Superstore dataset containing information about orders, customers, products, regions, shipping methods, sales, discounts, and profit. The goal is to identify data-quality issues, analyze business performance, answer relevant business questions, and generate meaningful insights using Python.

This project demonstrates essential skills required for a **Data Analyst**, including data assessment, data cleaning, exploratory data analysis, visualization, KPI calculation, and business interpretation.

---

## 🎯 Project Objectives

- Understand the structure and characteristics of the dataset
- Assess the quality and consistency of the data
- Identify missing values and duplicate records
- Check data types and invalid values
- Analyze sales and profit trends
- Compare categories and sub-categories
- Identify high-performing and low-performing products
- Analyze customer and regional performance
- Study shipping methods
- Understand the relationship between discount and profit
- Detect outliers and unusual observations
- Generate data-driven business insights

---

## 🗂️ Dataset Information

The Superstore dataset contains **9,994 records and 21 columns**.

### Important Columns

| Column | Description |
|---|---|
| Row ID | Unique row identifier |
| Order ID | Unique order identifier |
| Order Date | Date on which the order was placed |
| Ship Date | Date on which the order was shipped |
| Ship Mode | Shipping method |
| Customer ID | Unique customer identifier |
| Customer Name | Customer name |
| Segment | Customer segment |
| Country | Customer country |
| City | Customer city |
| State | Customer state |
| Postal Code | Postal or ZIP code |
| Region | Geographic region |
| Product ID | Unique product identifier |
| Category | Product category |
| Sub-Category | Product sub-category |
| Product Name | Product name |
| Sales | Sales amount |
| Quantity | Quantity ordered |
| Discount | Discount applied |
| Profit | Profit generated |

---

## 🛠️ Tools and Technologies

- **Python**
- **Pandas**
- **NumPy**
- **Matplotlib**
- **Seaborn**
- **Google Colab**
- **Jupyter Notebook**

---

## 🔍 Project Workflow

### 1. Data Understanding

The dataset is examined to understand its structure and contents.

Activities include:

- Importing the dataset
- Checking the number of rows and columns
- Viewing the first and last records
- Reviewing column names
- Checking data types
- Generating descriptive statistics
- Identifying categorical and numerical columns

### 2. Data Assessment

The dataset is checked for possible data-quality problems.

Assessment includes:

- Missing-value analysis
- Duplicate-record analysis
- Data-type validation
- Unique-value analysis
- Inconsistent category names
- Invalid numerical values
- Date consistency checks
- Repeated identifiers
- Outlier identification

### 3. Data Cleaning

The data is prepared for reliable analysis.

Possible cleaning activities include:

- Converting date columns into datetime format
- Handling missing values
- Reviewing duplicate records
- Standardizing categorical values
- Validating numerical columns
- Checking discount, sales, quantity, and profit values
- Creating analysis-ready columns

### 4. Exploratory Data Analysis

#### Sales Analysis

- Sales distribution
- Yearly sales performance
- Monthly sales trends
- Sales by category
- Sales by sub-category
- Top products by sales

#### Profit Analysis

- Profit distribution
- Yearly profit performance
- Profit by category
- Profit by sub-category
- Top and bottom products by profit

#### Customer Analysis

- Customer-wise sales
- Customer-wise profit
- Segment-wise performance
- Top customers by sales
- Top customers by profit

#### Geographic Analysis

- Sales by region
- Profit by region
- State-wise sales
- State-wise profit
- City-level performance

#### Shipping Analysis

- Order count by shipping mode
- Sales by shipping mode
- Profit by shipping mode
- Shipping performance comparison

#### Discount Analysis

- Discount distribution
- Discount versus profit
- Profitability at different discount levels
- Identification of heavily discounted products or categories

---

## 📈 Visualizations

The project includes or can include the following visualizations:

- Sales Distribution
- Yearly Sales and Profit
- Monthly Sales Trend
- Profit by Category
- Sales by Category
- Sub-Category Performance
- Top Products by Sales
- Top Products by Profit
- Regional Sales and Profit
- Customer Performance
- Shipping Mode Analysis
- Discount versus Profit
- Correlation Heatmap
- Outlier Analysis

Each visualization should be supported by a short interpretation describing its business relevance.

---

## ❓ Business Questions

The project aims to answer the following questions:

1. How do sales and profit change over time?
2. Which category generates the highest sales?
3. Which category generates the highest profit?
4. Which sub-categories perform well or poorly?
5. Which products generate the highest sales?
6. Which products generate the highest profit?
7. Which regions contribute the most sales and profit?
8. Which customer segments perform best?
9. Which customers contribute the most revenue?
10. Which shipping modes are most frequently used?
11. What relationship exists between discount and profit?
12. Are there products with high sales but low profit?
13. Which areas require further business investigation?

---

## 📊 Key Performance Indicators

| KPI | Description |
|---|---|
| Total Sales | Sum of all sales values |
| Total Profit | Sum of all profit values |
| Total Orders | Number of unique orders |
| Total Customers | Number of unique customers |
| Total Quantity | Total quantity sold |
| Average Order Value | Total sales divided by unique orders |
| Profit Margin | Total profit divided by total sales × 100 |
| Average Discount | Average discount across transactions |

### Example KPI Code

```python
total_sales = df["Sales"].sum()

total_profit = df["Profit"].sum()

total_orders = df["Order ID"].nunique()

total_customers = df["Customer ID"].nunique()

total_quantity = df["Quantity"].sum()

profit_margin = (total_profit / total_sales) * 100
```

---

## 💡 Initial Business Observations

The exploratory analysis includes the following observations:

- Sales values are highly right-skewed, with many lower-value transactions and fewer high-value transactions.
- Yearly analysis shows changes in sales and profit over the analyzed period.
- Technology and Office Supplies show substantial profit contributions in the category analysis.
- Furniture contributes comparatively less profit than the other displayed categories.
- High sales do not necessarily result in high profitability.
- Discount levels should be analyzed together with profit to understand their possible business impact.

These observations should be supported with calculated values and additional analysis in the notebook.

---

## 📁 Project Structure

```text
Superstore-Sales-Assessment/
│
├── superstoreeda.ipynb
├── README.md
├── dataset/
│   └── superstore.csv
│
├── visualizations/
│   ├── sales_distribution.png
│   ├── yearly_sales_profit.png
│   ├── monthly_sales.png
│   └── category_profit.png
│
└── requirements.txt
```

---

## ▶️ How to Run the Project

### Using Google Colab

1. Open the notebook in Google Colab.
2. Upload the dataset or connect Google Drive.
3. Update the dataset path if required.
4. Run the notebook cells sequentially.
5. Review the results, visualizations, and business insights.

### Using Jupyter Notebook

Install the required libraries:

```bash
pip install pandas numpy matplotlib seaborn jupyter
```

Launch Jupyter Notebook:

```bash
jupyter notebook
```

Open the project notebook:

```text
superstoreeda.ipynb
```

---

## 🧠 Skills Demonstrated

- Data Assessment
- Data Cleaning
- Data Validation
- Exploratory Data Analysis
- Data Visualization
- Statistical Analysis
- KPI Calculation
- Business Question Formulation
- Business Insight Generation
- Python Programming
- Pandas and NumPy
- Matplotlib and Seaborn

---

## 🚀 Future Improvements

- Build an interactive Power BI dashboard
- Perform RFM customer segmentation
- Develop sales and profit forecasting
- Perform customer lifetime value analysis
- Build predictive machine-learning models
- Create a web-based analytics dashboard
- Add automated data-quality checks
- Compare business performance with predefined targets

---

## 👨‍💻 Author

**Shoheb Mulla**

### Skills

`Python` `Pandas` `NumPy` `Matplotlib` `Seaborn` `EDA` `Data Assessment` `Data Cleaning` `Data Visualization` `Business Analytics`

---

## 📌 Project Outcome

This project demonstrates the ability to:

1. Understand raw business data.
2. Assess data quality and identify inconsistencies.
3. Clean and prepare data for analysis.
4. Perform exploratory data analysis.
5. Create meaningful visualizations.
6. Calculate important business KPIs.
7. Answer business questions using data.
8. Communicate insights in a structured manner.
