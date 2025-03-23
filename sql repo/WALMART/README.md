Walmart Sales Data Exploratory Data Analysis (EDA) using SQL

📌 Project Overview

This project involves performing exploratory data analysis (EDA) on Walmart sales data using SQL. The objective is to derive insights from sales transactions, understand customer purchasing patterns, and analyze product performance across different stores.

🛠️ Tools & Technologies

Database Management System: MySQL / PostgreSQL / SQL Server (as applicable)

SQL Queries: Used for data extraction, cleaning, and analysis

📂 Dataset Overview

The dataset contains transactional sales data for Walmart, including:

Invoice ID: Unique identifier for each transaction

Branch: Store location identifier

Customer Type: Regular vs. Member

Product Line: Category of purchased products

Unit Price: Price per unit of the product

Quantity: Number of units sold

Tax 5%: Tax amount applied to the purchase

Total: Final price after tax

Date: Transaction date

Payment Method: Cash, Credit Card, or E-Wallet

Customer Rating: Satisfaction rating provided by customers

🔍 Analysis Performed

Sales Trends: Identified total sales per branch and monthly trends.

Customer Insights: Analyzed customer purchase behavior and preferences.

Product Performance: Determined the best-selling product lines.

Revenue Analysis: Computed total revenue and tax contributions.

Payment Methods: Evaluated the most popular modes of payment.

📜 SQL Queries

The project includes various SQL queries for data analysis, such as:

-- Total sales per branch
SELECT Branch, SUM(Total) AS Total_Sales
FROM walmart_sales
GROUP BY Branch
ORDER BY Total_Sales DESC;

-- Best-selling product lines
SELECT Product_Line, COUNT(*) AS Total_Sales
FROM walmart_sales
GROUP BY Product_Line
ORDER BY Total_Sales DESC;

-- Most popular payment method
SELECT Payment, COUNT(*) AS Payment_Count
FROM walmart_sales
GROUP BY Payment
ORDER BY Payment_Count DESC;

📊 Key Findings

Branch X had the highest total sales, whereas Branch Y had the lowest.

E-Wallets were the most preferred payment method.

The "Health and Beauty" product line had the highest sales volume.

The majority of customers were regular buyers, but members tended to spend more per transaction.

📁 Repository Structure

SQL-repo/
├── WALMART/
│   ├── walmartsalesEDA.sql  # SQL script containing queries
│   ├── walmart_sales.csv     # Raw dataset (if applicable)
│   ├── README.md             # Project documentation

🚀 How to Use

Clone this repository:

git clone https://github.com/nishanthnirujogi/SQL-repo.git

Load the dataset into your preferred SQL database.

Run the walmartsalesEDA.sql script to perform the analysis.

Modify or expand queries to gain additional insights.

📌 Future Enhancements

Advanced Data Visualization: Use Power BI/Tableau for dashboard reporting.

Predictive Analytics: Apply ML models to forecast sales.

Customer Segmentation: Cluster customers based on purchase behavior.

📧 Contact

For any queries, feel free to reach out:

Name: Nirujogi Nisanth

Email: nirujoginisanth@gmail.com

GitHub: nishanthnirujogi
