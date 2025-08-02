# Walmart-Sales-Analysis
End-to-end data analysis of Walmart sales using Python for cleaning, SQL for querying, and structured problem-solving to derive business insights. Ideal for analysts seeking hands-on experience with data pipelines, SQL logic, and real-world analytical thinking.

1. Set Up the Environment

Tools Used: Visual Studio Code (VS Code), Python, MySQLGoal: Create a structured workspace in VS Code and organize folders for smooth development.

2. Set Up Kaggle API

Get your Kaggle API token from profile settings (kaggle.json)

Save it in your local .kaggle folder

Download datasets using:kaggle datasets download -d <dataset-path>

3. Download Walmart Sales Data

Source: Kaggle Walmart Sales Dataset

Store: Save inside data/ folder

4. Install Required Libraries and Load Data

Install using:

pip install pandas numpy sqlalchemy mysql-connector-python

Then load data into a Pandas DataFrame.

5. Explore the Data

Use functions like .info(), .describe(), and .head() to:

Understand structure

Check column names, types, distributions

6. Data Cleaning

Duplicates: Drop them

Missing Values: Drop or impute

Fix Data Types: Ensure correct formats (e.g., dates, currency)

Currency Formatting: Use .replace() for cleanup

Validation: Confirm consistency

7. Feature Engineering

Create Total Amount = unit_price * quantity

This supports later SQL aggregation and analysis

8. Load Data into MySQL

Use sqlalchemy to connect to MySQL and upload the DataFrame

Automate table creation and insertion using Python

9. SQL Analysis: Business Problem Solving

Key questions:

Revenue by branch/category

Best-selling products

Time-based sales trends

Preferred payment methods

Customer behavior and peak periods

Document: Keep notes on each query's objective and result

10. Project Publishing and Documentation

Docs: README.md and Jupyter Notebooks

GitHub: Upload scripts, queries, notebooks, and explain data access

Requirements

Python: 3.8+

SQL Database: MySQL

Libraries: pandas, numpy, sqlalchemy, mysql-connector-python

Kaggle API Key: Required

Getting Started

git clone <repo-url>
pip install -r requirements.txt

Download data using Kaggle API, then process using main.py or notebooks

Project Structure

|-- data/              # Raw and cleaned data
|-- sql_queries/       # SQL scripts
|-- notebooks/         # Jupyter notebooks
|-- README.md          # Project documentation
|-- requirements.txt   # Required libraries
|-- main.py            # Main processing script

Results and Insights

Sales Insights: Key branches, categories, and payment modes

Profitability: Most profitable categories/branches

Customer Behavior: Ratings, timing, preferences

Future Enhancements

Add dashboards (Power BI, Tableau)

Pull from more data sources

Automate pipeline for real-time use

License

MIT License

Acknowledgments

Data: Kaggle Walmart Sales Dataset

Inspiration: Walmart case studies
