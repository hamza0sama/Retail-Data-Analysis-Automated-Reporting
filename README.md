# Mini-Project-001 | Advanced Python Data Exploration & Automated Reporting

## 📌 Project Overview

This project presents an end-to-end data analysis workflow for a retail business using the **Sample-Superstore2019** dataset.

The analysis focuses on understanding sales performance, profitability, customer behavior, product performance, discount impact, shipping operations, and business trends.

The project was developed using Python and Jupyter Notebook, with Pandas used for data manipulation and Matplotlib and Seaborn used for exploratory data analysis and visualization.

---

## 🏢 Business Scenario

A multinational retail company wants to analyze its sales data to better understand:

* Sales performance
* Profitability
* Customer segments
* Product performance
* Regional performance
* Discount impact
* Shipping behavior
* Sales and profit trends

The goal is to transform raw retail data into meaningful business insights that can support data-driven decision-making.

---

## 🎯 Project Objectives

The main objectives of this project are:

* Import and inspect the retail dataset.
* Check the structure and quality of the data.
* Handle data-quality issues.
* Perform exploratory data analysis.
* Analyze numerical and categorical variables.
* Investigate relationships between sales, profit, quantity, and discount.
* Analyze sales and profit trends over time.
* Identify high-performing products, customers, regions, and categories.
* Investigate the effect of discounts on profitability.
* Analyze shipping-mode usage.
* Create meaningful visualizations.
* Generate business insights from the analysis.
* Export the cleaned dataset for further use.

---

## 📊 Dataset

**Dataset:** `Sample-Superstore2019`

The dataset contains retail transaction data covering different aspects of the business, including:

* Orders
* Customers
* Products
* Categories
* Sub-Categories
* Sales
* Quantity
* Discount
* Profit
* Shipping information
* Customer segments
* Geographic information

The dataset is used to investigate business performance and identify important patterns and opportunities.

---

## 🛠️ Technologies & Libraries

The project was developed using:

* **Python**
* **Jupyter Notebook**
* **Pandas**
* **NumPy**
* **Matplotlib**
* **Seaborn**
* **PyArrow**

### Main uses

| Library    | Purpose                        |
| ---------- | ------------------------------ |
| Pandas     | Data manipulation and analysis |
| NumPy      | Numerical operations           |
| Matplotlib | Data visualization             |
| Seaborn    | Statistical visualization      |
| PyArrow    | Parquet data storage           |

---

# 🔄 Project Workflow

The project follows the following analytical workflow:

```text
Raw Dataset
     ↓
Data Loading
     ↓
Data Inspection
     ↓
Data Cleaning & Validation
     ↓
Feature Preparation
     ↓
Exploratory Data Analysis
     ↓
Statistical Analysis
     ↓
Correlation Analysis
     ↓
Business Analysis
     ↓
Data Visualization
     ↓
Business Insights
     ↓
Export Cleaned Dataset
```

---

# 🧹 Data Cleaning & Validation

The dataset was inspected to identify potential data-quality issues before performing the analysis.

The workflow includes checks for:

* Missing values
* Duplicate records
* Data types
* Dataset structure
* Numerical variables
* Categorical variables
* Potential outliers
* Distribution characteristics

The cleaned dataset was then stored in **Parquet format** for efficient storage and later analysis.

```python
df.to_parquet("cleaned_data.parquet", engine="pyarrow")
```

---

# 🔎 Exploratory Data Analysis

The project performs exploratory analysis on both numerical and categorical variables.

### Numerical Analysis

The following variables were investigated:

* Sales
* Profit
* Quantity
* Discount

For numerical variables, the analysis includes:

* Descriptive statistics
* Distribution analysis
* Skewness
* Kurtosis where relevant
* Histogram analysis
* Boxplot analysis

---

# 📊 Distribution Analysis

The distributions of Sales, Profit, and Discount were analyzed using histograms and boxplots.

### Sales

Sales distribution was examined to understand its spread and identify potential extreme values.

### Profit

Profit distribution was analyzed to understand profitability patterns and potential negative-profit observations.

### Discount

Discount was analyzed as a discrete numerical variable with several predefined discount levels.

The analysis showed that discounts are concentrated around specific values, with no-discount orders representing a large portion of the dataset.

---

# 🔗 Correlation Analysis

A correlation matrix was created for:

* Sales
* Profit
* Quantity
* Discount

A correlation heatmap was used to visualize the relationships between these variables.

### Key Findings

* **Sales and Profit** show a moderate positive correlation.
* **Discount and Profit** show a negative correlation, suggesting that higher discounts tend to reduce profitability.
* **Quantity and Sales** show a weak positive relationship.

---

# 📦 Categorical Analysis

The following categorical variables were analyzed:

* Category
* Sub-Category
* Segment
* Region
* Ship Mode

Their distributions were visualized to understand the composition of the dataset and customer/business activity.

---

# 💰 Sales Analysis

Sales performance was analyzed across multiple business dimensions.

### Sales by Category

The total sales generated by each product category were calculated and visualized.

### Top 10 Products by Sales

The top products were identified based on total sales.

The analysis showed that:

**Canon imageCLASS 2200 Advanced Copier**

was the highest-selling product in terms of total sales.

### Top 10 Customers by Sales

Customers were ranked based on their total sales contribution.

### Sales by Region

Regions were compared using total sales and average sales.

The **West region** generated the highest total sales.

---

# 📈 Profit Analysis

Profitability was analyzed across different business dimensions.

The analysis includes:

* Profit by Category
* Profit by Segment
* Profit by Product
* Profit by Customer
* Profit by Region
* Profit by Year
* Profit by Month

The project also identifies products generating negative total profit.

---

# 👥 Customer Segment Analysis

Customer segments were compared using sales and average sales.

The three main segments are:

* Consumer
* Corporate
* Home Office

### Key Finding

**Consumer** generated the highest total sales, while **Home Office** had the highest average sales per order.

This indicates that total revenue and average transaction value can tell different stories about customer behavior.

---

# 🌎 Regional Analysis

Regional performance was analyzed using:

* Total Sales
* Average Sales
* Total Profit
* Average Profit

### Key Finding

**West** was the strongest region based on total sales and total profit.

The analysis also highlighted differences between total performance and average transaction performance across regions.

---

# 🏷️ Discount Analysis

Discount levels were categorized into:

* No Discount
* Low Discount
* Medium Discount
* High Discount
* Very High Discount

The analysis compared sales and profitability across these levels.

### Key Findings

* Orders with **no discount** generated the highest total sales and total profit.
* Low discounts remained profitable.
* Medium, High, and Very High discount levels generated negative total profit.
* Medium discounts produced the highest average sales per order but resulted in negative average profit.

### Business Implication

Higher discounts do not necessarily lead to better profitability. Discount strategies should therefore be evaluated based on both revenue and profit rather than sales alone.

---

# 🚚 Shipping Analysis

Shipping modes were analyzed based on the number of orders.

The available shipping modes include:

* Standard Class
* Second Class
* First Class
* Same Day

### Key Finding

**Standard Class** was the most frequently used shipping mode, with **5,967 orders**.

Same Day shipping had the lowest usage, with **543 orders**.

---

# 📅 Time Trend Analysis

Sales and profit were analyzed across:

* Years
* Months

## Sales by Year

The analysis showed that:

* 2017 experienced a slight decline compared with 2016.
* Sales increased significantly in 2018.
* **2019 recorded the highest annual sales.**

## Monthly Analysis

Monthly sales and profit trends were visualized to identify seasonal patterns and high-performing periods.

---

# 🗺️ State-Level Analysis

The top states were ranked according to total sales.

### Top Revenue-Generating States

1. California
2. New York
3. Texas
4. Washington
5. Pennsylvania

### Important Finding

Although **Texas** ranked among the highest states in total sales, it generated negative total profit.

This demonstrates why analyzing revenue alone is insufficient for evaluating business performance.

---

# ⚠️ High-Sales but Low/Negative-Profit Products

The project identifies products that generate relatively high sales but have zero or negative total profit.

Examples include:

* Cisco TelePresence System EX90 Videoconferencing Unit
* GBC DocuBind P400 Electric Binding System
* Lexmark MX611dhe Monochrome Laser Printer
* Cubify CubeX 3D Printer Double Head Print

### Business Implication

High revenue does not necessarily mean high profitability.

These products should be investigated further to determine whether pricing, discounts, costs, or other operational factors are responsible for their low profitability.

---

# 📊 Visualizations

The project includes more than the required minimum of **8 visualizations**.

The visual analysis includes:

1. Correlation Heatmap
2. Sales Distribution
3. Sales Boxplot
4. Profit Distribution
5. Profit Boxplot
6. Discount Distribution
7. Discount Boxplot
8. Category Distribution
9. Sub-Category Distribution
10. Segment Distribution
11. Region Distribution
12. Shipping Mode Distribution
13. Total Sales by Category
14. Top 10 Products by Sales
15. Top 10 Products by Profit
16. Total Profit by Category
17. Total Profit by Segment
18. Top 10 Customers by Profit
19. Top 10 Customers by Sales
20. Monthly Sales Trend
21. Monthly Profit Trend
22. Sales by Year
23. Profit by Year

These visualizations provide both statistical and business-oriented perspectives on the dataset.

---

# 💡 Key Business Insights

The analysis produced several important findings:

### 1. Consumer Segment Dominates Revenue

Consumer customers generate the highest total sales among the analyzed customer segments.

### 2. West Is the Strongest Region

The West region generates the highest total sales and total profit.

### 3. Discounts Can Damage Profitability

Higher discount levels are associated with significantly lower profitability, with several discount categories generating negative profit.

### 4. Revenue Does Not Always Mean Profit

Some products and states generate high sales but negative profit, demonstrating the importance of profitability analysis.

### 5. Standard Shipping Is Dominant

Standard Class is by far the most frequently used shipping mode.

### 6. 2019 Was the Strongest Sales Year

2019 recorded the highest total annual sales in the analyzed period.

### 7. High-Value Orders Can Exist in Lower-Revenue Segments

Home Office generated lower total sales than Consumer and Corporate but had a higher average sales value per order.

---

# 💾 Data Export

After the cleaning and preprocessing workflow, the resulting dataset was exported as a Parquet file:

```text
cleaned_data.parquet
```

Parquet was selected as an efficient format for storing and loading the processed DataFrame.

---

# 📓 Notebook Documentation

The complete workflow is documented in Jupyter Notebook.

The notebooks cover:

* Data loading
* Data inspection
* Data validation
* Exploratory data analysis
* Statistical analysis
* Correlation analysis
* Business questions
* Visualizations
* Business insights
* Data export

---

# 📁 Project Structure

```text
Mini-Project-001/
│
├── README.md
│
├── notebooks/
│   ├── Data_Cleaning.ipynb
│   ├── Business_Analysis.ipynb
│   └── EDA_Visualization.ipynb
│
├── data/
│   └── cleaned_data.parquet
│
└── requirements.txt
```

> The exact file names and folder structure can be adjusted to match the final GitHub repository.

---

# 🚀 How to Run

### 1. Install the required libraries

```bash
pip install pandas numpy matplotlib seaborn pyarrow jupyter
```

### 2. Launch Jupyter Notebook

```bash
jupyter notebook
```

### 3. Open the project notebooks

Run the notebooks in the appropriate order, starting with the data preparation notebook and then continuing with the analysis and visualization notebooks.

---

# 🏁 Conclusion

This project demonstrates an end-to-end retail data analysis workflow using Python.

The analysis transforms the **Sample-Superstore2019** dataset into actionable business insights through data validation, exploratory analysis, statistical analysis, correlation analysis, visualization, and business-focused investigation.

The results demonstrate that evaluating retail performance requires looking beyond sales alone and considering **profitability, discounts, customer segments, products, regions, shipping behavior, and time trends**.

The project provides a practical foundation for understanding retail performance and supporting data-driven business decisions.

---

## 👨‍💻 Author

**Hamza Osama Aboshady**

Data Science Student | Data Analyst

Alexandria University
