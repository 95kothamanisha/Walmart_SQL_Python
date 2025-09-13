# Walmart Data Analysis: End-to-End SQL + Python Project 

## Project Overview
<img width="1598" height="753" alt="image" src="https://github.com/user-attachments/assets/3eafe932-e512-4fe9-9a65-f6a22df3a903" />


I worked on an end-to-end data analysis project using **Python and SQL** on Walmart sales data.
The main goal of my project was to **extract business insights** such as sales performance, customer buying behavior, and profitability.
I structured my work like a pipeline — starting from data collection, cleaning, and transformation, all the way to SQL-based problem solving and insights generation.

---

## Project Steps

### 1. Setting Up the Environment

I used **VS Code** as my workspace, and I worked with both **Python and SQL (MySQL/PostgreSQL)**.
I created a structured folder system for data, SQL scripts, and documentation so that everything stayed organized.

### 2. Kaggle API Setup

I connected to Kaggle by generating an API token and placing it in the `.kaggle` folder.
This allowed me to download datasets directly using the Kaggle API.

### 3. Data Collection

I downloaded the **Walmart Sales Dataset** from Kaggle and stored it in the `data/` folder for easy access.

### 4. Installing Libraries & Loading Data

I installed libraries like **pandas, numpy, sqlalchemy, mysql-connector-python, psycopg2**.
Then, I loaded the dataset into a **Pandas DataFrame** for initial exploration.

### 5. Data Exploration

I explored the data using `.head()`, `.info()`, and `.describe()` to understand the structure, data types, and any irregularities.

### 6. Data Cleaning

I removed duplicates, handled missing values, and fixed data types.
For example, I converted `date` to `datetime` and `unit_price` to `float`.
I also ensured that all values were consistent and valid.

### 7. Feature Engineering

I created a **new column `Total Amount`**, calculated as `unit_price × quantity`.
This made it easier to analyze revenue and profit in SQL.

### 8. Loading Data into Databases

I used **SQLAlchemy** to connect to MySQL and PostgreSQL.
I created tables automatically and loaded the cleaned dataset into both databases.
After loading, I verified with queries like `SELECT COUNT(*)` to ensure the data was properly inserted.

### 9. SQL Analysis – Solving Business Problems

This was the main part of my project. I wrote SQL queries to answer key questions, such as:

* Which categories and branches generate the most revenue?
* What are the most preferred **payment methods**?
* Which days and time periods are the busiest?
* How does profitability vary by branch and category?
* Which branches experienced a revenue decrease compared to last year?

I made use of **aggregate functions, window functions, GROUP BY, CTEs, and joins** to perform complex analysis.

### 10. Documentation & Publishing

Finally, I documented the entire workflow in a **README file** and organized everything into folders:

* `data/` for raw and cleaned datasets
* `sql_queries/` for SQL scripts
* `notebooks/` for Python Jupyter analysis
* `main.py` for main data processing pipeline

I also planned to publish the project on **GitHub** with clear documentation.

---

## Results and Insights

From the analysis, I was able to identify:

* **Sales Insights**: Best-performing branches and categories, along with customer-preferred payment methods.
* **Profitability**: The most profitable categories and cities.
* **Customer Behavior**: Trends in ratings, shopping hours, and seasonal buying patterns.

---

## Future Enhancements

To make this project more powerful, I considered:

* Creating dashboards in **Power BI / Tableau** for visualization.
* Automating the data pipeline for **real-time data updates**.
* Including additional datasets for deeper insights.


## Acknowledgments
* Data Source: Kaggle’s Walmart Sales Dataset
* Inspiration: Walmart’s business case studies on sales and supply chain optimization.

