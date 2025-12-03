# Data Analytics Project – Python, SQL & Power BI

# Customer Shopping Behavior Analysis

## Overview
This project analyzes customer shopping behavior for a retail business using an end-to-end data analytics workflow.  
It starts with raw transactional data in CSV format, moves through Python-based EDA and cleaning, uses MySQL for structured analysis with SQL, and finishes with an interactive Power BI dashboard and business recommendations.

The goal is to show how I can turn raw customer data into clear, actionable insights for marketing, product, and strategy teams.

---

## Dataset
- **File:** `customer_shopping_behavior.csv`  
- **Size:** 3,900 purchases, 18 columns  
- **Key fields:**
  - Customer: age, gender, location, subscription status  
  - Purchase: item purchased, category, purchase amount, season, size, color  
  - Behavior: discount applied, previous purchases, frequency of purchases, review rating  
  - Logistics: shipping type  

Missing values (mainly in review ratings) are handled during the cleaning step in Python.

---

## Tools & Technologies
- **Python** – data loading, EDA, cleaning  
  - Notebook: `Customer_Shopping_Behavior_Analysis.ipynb`
- **Database:** MySQL Server  
  - Queries: `customer_behavior_sql_queries.sql`
- **Visualization:** Power BI  
  - Dashboard: `customer_behavior_dashboard.pbix`
- **Documentation:**  
  - `Business Problem Document.pdf`  
  - `Customer Shopping Behavior Analysis.pdf`  
  - `Customer-Shopping-Behavior-Analysis.pptx`

---

## Project Steps

1. **Load & Explore Data (Python)**
   - Import the CSV into a Pandas DataFrame.
   - Inspect data types, missing values, and basic statistics.
   - Understand customer and purchase distributions.

2. **EDA (Exploratory Data Analysis)**
   - Analyze spending patterns by age, gender, category, and season.
   - Explore relationships between discounts, reviews, subscriptions, and spend.
   - Visualize key trends (histograms, bar charts, correlations).

3. **Data Cleaning & Preparation**
   - Handle missing review ratings (e.g., median by category).
   - Standardize column names and formats.
   - Remove duplicates and fix inconsistent values.
   - Create features such as age groups and purchase frequency.

4. **SQL Analysis in MySQL**
   - Load the cleaned dataset from Python into a MySQL table.
   - Use `customer_behavior_sql_queries.sql` to answer business questions, such as:
     - Revenue by gender and age group  
     - High-spending customers using discounts  
     - Top-rated and most-purchased products  
     - Standard vs. express shipping behavior  
     - Subscribers vs. non-subscribers and customer segments (New, Returning, Loyal)

5. **Power BI Dashboard**
   - Connect Power BI to the MySQL database (or cleaned CSV export).
   - Build visuals for revenue, orders, and ratings by key segments.
   - Add slicers for gender, category, shipping type, age group, and subscription status.

---

## Dashboard
The **Customer Behavior Dashboard** highlights:

- **KPI cards:** number of customers, average purchase amount, average review rating  
- **Subscription view:** share of customers who subscribe vs. non-subscribers  
- **Category performance:** revenue and sales by product category  
- **Age group insights:** revenue and sales by age group  
- **Shipping comparison:** difference in spend between standard and express shipping  

The layout is designed to be clean and business-friendly, so non-technical stakeholders can quickly explore customer segments and performance.

---

## Results & Business Insights
Key findings from the analysis include:

- Certain age groups contribute a higher share of total revenue.  
- Subscribers and frequent buyers tend to spend more and show stronger loyalty.  
- Express shipping customers generally have higher average order values than standard shipping users.  
- A small set of top-rated and most-purchased products drives a significant portion of revenue.  

Based on these insights, recommendations include strengthening subscription and loyalty programs, targeting high-value segments with personalized offers, promoting top-rated products, and optimizing discount strategies.

---

## How to Run the Project

1. **Clone or download the project files** into a local folder.

2. **Run the Python notebook**
   - Open `Customer_Shopping_Behavior_Analysis.ipynb` in Jupyter or VS Code.
   - Run all cells to:
     - Load the CSV
     - Perform EDA and cleaning
     - Export the cleaned dataset or load it directly into MySQL

3. **Set up MySQL**
   - Create a new database (e.g., `customer_behavior`).
   - Create a table and load the cleaned data.
   - Open `customer_behavior_sql_queries.sql` in your SQL client and run the queries to reproduce the analysis.

4. **Open the Power BI dashboard**
   - Open `customer_behavior_dashboard.pbix` in Power BI Desktop.
   - Update the data source to point to your MySQL database (or cleaned CSV).
   - Refresh the data to interact with the latest results.

This project is structured to be easy for recruiters and hiring managers to review, while clearly demonstrating practical skills in Python, SQL, and Power BI applied to a real business problem.
