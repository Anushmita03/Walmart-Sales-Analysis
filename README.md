# 🛒 Walmart Sales Data Analysis

## 📌 Project Overview

This project is an end-to-end data analysis of Walmart sales using Python for cleaning, SQL for querying, and structured problem-solving to derive business insights. It uses Python, MySQL, and SQLAlchemy to handle data processing, storage, and complex query analysis.


---

## 🚀 Project Steps

### 1. Set Up the Environment

* **Tools Used:** VS Code, Python, MySQL
* **Goal:** Organize workspace and set up development environment.

### 2. Set Up Kaggle API

* Downloaded `kaggle.json` from Kaggle account settings.
* Placed it in the `.kaggle` folder on our system.
* Used:

  ```bash
  kaggle datasets download -d <dataset-path>
  ```

  to download data.

### 3. Download Walmart Sales Data

* Data Source: Used the Kaggle API to download the Walmart sales datasets from Kaggle.
* Dataset Link: [Walmart Sales Dataset](https://www.kaggle.com/datasets/najir0123/walmart-10k-sales-datasets)
* Saved the dataset in the `data/` folder.

### 4. Install Required Libraries & Load Data

Libraries: Installed necessary Python libraries using:
```bash
pip install pandas numpy sqlalchemy mysql-connector-python
```

* Loading Data: Read the data into a Pandas DataFrame for initial analysis and transformations.

### 5. Data Exploration

* Goal: Conducted an initial data exploration to understand data distribution, check column names, types, and identify potential issues.
* Analysis: Used functions like `.info()`, `.describe()`, `.head()` to explore the data.

### 6. Data Cleaning

* Remove Duplicates: Identified and removed duplicate entries to avoid skewed results.
* Handle Missing Values: Dropped rows or columns with missing values if they are insignificant; fill values where essential.
* Fix Data Types: Ensured all columns have consistent data types (e.g., dates as datetime, prices as float).
* Currency Formatting: Used .replace() to handle and format currency values for analysis.
* Validation: Checked for any remaining inconsistencies and verify the cleaned data.

### 7. Feature Engineering

* Create New Columns: Calculated the Total Amount for each transaction by multiplying unit_price by quantity and adding this as a new column( `Total Amount` column = `unit_price * quantity`)
* Enhance Dataset: Adding this calculated field streamlined further SQL analysis and aggregation tasks.

### 8. Load Data into MySQL

* Set Up Connections: Connected to MySQL using sqlalchemy and load the cleaned data into each database.
* Table Creation: Set up tables in MySQL using Python SQLAlchemy to automate table creation and data insertion.
* Verification: Ran initial SQL queries to confirm that the data has been loaded accurately.

### 9. SQL Analysis

Business Problem-Solving: Wrote and executed complex SQL queries to answer critical business questions, such as:
* Revenue trends across branches and categories.
* Identifying best-selling product categories.
* Sales performance by time, city, and payment method.
* Analyzing peak sales periods and customer buying patterns.
* Create tables and insert cleaned data
* Profit margin analysis by branch and category.
Documentation: Kept clear notes of each query's objective, approach, and results.
---

## 📂 Project Structure

```
|-- data/               # Raw and cleaned data
|-- sql_queries/        # SQL scripts
|-- notebooks/          # Jupyter notebooks
|-- README.md           # Documentation
|-- requirements.txt    # Required Python libraries
|-- main.py             # Script for loading and processing
```

---

## ✅ Requirements

* Python 3.8+
* MySQL
* Libraries: `pandas`, `numpy`, `sqlalchemy`, `mysql-connector-python`
* Kaggle API key

---

## 📈 Results & Insights

* **Top Products:** High revenue categories
* **Best Branches:** Sales & profitability
* **Customer Behavior:** Rating trends, popular payment modes, peak hours

---

## 🔧 Future Enhancements

* Integration with a dashboard tool (e.g., Power BI or Tableau) for interactive visualization.
* Additional data sources to enhance analysis depth.
* Automation of the data pipeline for real-time data ingestion and analysis.

---

## 📄 License

This project is licensed under the MIT License.

---

## 🙌 Acknowledgments

* **Data Source:** [Kaggle – Walmart Sales Dataset]([https://www.kaggle.com/datasets](https://www.kaggle.com/datasets/najir0123/walmart-10k-sales-datasets))
* **Inspiration:** Walmart’s business case studies on sales and supply chain optimization.

---
