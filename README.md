# Advanced Python Data Exploration & Automated Reporting

##  Project Overview

An end-to-end **retail data analysis project** using the **Sample-Superstore2019** dataset.

The project focuses on sales, profitability, customer behavior, product performance, discounts, shipping, regional performance, and business trends using Python and Jupyter Notebook.

##  Objectives

* Clean and validate the dataset
* Perform exploratory and statistical analysis
* Analyze sales, profit, quantity, and discount
* Identify top products, customers, categories, and regions
* Analyze discount impact on profitability
* Explore shipping and time trends
* Create meaningful visualizations
* Generate business insights
* Export the cleaned dataset

##  Technologies

* Python
* Jupyter Notebook
* Pandas
* NumPy
* Matplotlib
* Seaborn
* PyArrow

##  Workflow

```text
Raw Data
   ↓
Data Inspection
   ↓
Data Cleaning & Validation
   ↓
EDA & Statistical Analysis
   ↓
Correlation Analysis
   ↓
Business Analysis
   ↓
Visualization
   ↓
Business Insights
   ↓
Cleaned Data Export
```

##  Key Insights

* **Consumer** generated the highest total sales.
* **West** was the strongest region in total sales and profit.
* Higher discounts were associated with lower profitability.
* Some high-sales products and states generated negative profit.
* **Standard Class** was the most frequently used shipping mode.
* **2019** recorded the highest annual sales.
* **Home Office** had a higher average sales value per order despite lower total sales.

##  Data Export

The cleaned dataset was exported in **Parquet** format:

```text
cleaned_data.parquet
```

##  Project Structure

```text
Mini-Project-001/
│
├── README.md
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

##  How to Run

Install the required libraries:

```bash
pip install pandas numpy matplotlib seaborn pyarrow jupyter
```

Launch Jupyter Notebook:

```bash
jupyter notebook
```

Then run the notebooks in the appropriate order.

##  Conclusion

This project demonstrates a complete **Python-based retail data analysis workflow**, transforming raw data into actionable business insights.

It highlights why retail performance should be evaluated through **both sales and profitability**, while considering discounts, customers, products, regions, shipping, and time trends.

##  Author

**Hamza Osama Aboshady**

Data Science Student | Data Analyst
Alexandria University
