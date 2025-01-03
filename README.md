Marketing Insights with Machine Learning for E-Commerce Business
Business Context
This project is built to analyze marketing insights for a leading e-commerce company to help define future marketing strategies. The main goal is to understand the business performance through a detailed analysis of transactions, customer behavior, marketing spend, and other key performance indicators (KPIs). Additionally, the company aims to develop an analytical dashboard to monitor various KPIs and business metrics.

Available Data
The project uses the following datasets from the e-commerce company, covering the period from January 1, 2019, to December 31, 2019:

Online_Sales.csv
Contains transaction-level data from the point of sale, including:

CustomerID: Unique ID of the customer
Transaction_ID: Unique ID of the transaction
Transaction_Date: Date of the transaction
Product_SKU: SKU ID for the product
Product_Description: Product description
Product_Category: Category of the product
Quantity: Number of items ordered
Avg_Price: Price per unit
Delivery_Charges: Charges for delivery
Coupon_Status: Whether a discount coupon was applied
Customers_Data.csv
Contains customer demographics:

CustomerID: Unique ID of the customer
Gender: Gender of the customer
Location: Location of the customer
Tenure_Months: Duration of customer subscription in months
Discount_Coupon.csv
Details about discount coupons applied:

Month: Month the coupon was applied
Product_Category: Product category for the coupon
Coupon_Code: Coupon code applied
Discount_pct: Percentage of discount applied
Marketing_Spend.csv
Contains marketing spend details on both offline and online channels:

Date: Date of the marketing spend
Offline_Spend: Spend on offline channels (TV, Radio, NewsPapers, Billboards, etc.)
Online_Spend: Spend on online channels (Google Ads, Facebook, etc.)
Tax_Amount.csv
GST (Goods and Services Tax) details for different product categories:

Product_Category: Product category
GST: GST percentage for that category
Key Definitions
Invoice Value:
The total value of a transaction calculated using the formula:


Invoice Value = ((Quantity * Avg_Price) * (1 - Discount_pct) * (1 + GST)) + Delivery_Charges
Average Order Value (AOV):
The total revenue divided by the number of transactions per customer.

Profit Margin:
Profit margin is the percentage of total sales that has been earned as gain.

Purchase Frequency:
The average number of purchases made by a customer over a defined period, typically a month or year.

Repeat Rate:
The percentage of your customer base that has returned to make another purchase.

Churn Rate:
The percentage of customers who stop subscribing annually.

Customer Lifetime Value (CLV):
A prediction of the net profit generated from the entire future relationship with a customer.

Business Objective
1. Invoice Calculation and Revenue Analysis
Calculate the invoice amount for each transaction and item level using the formula above.
2. Exploratory Data Analysis (EDA)
Analyze customer acquisition on a monthly basis.

Understand customer retention month-on-month.

Measure revenue from new vs. existing customers.

Analyze the impact of discounts on revenue.

Explore KPIs such as revenue, number of orders, average order value, quantity sold, etc., categorized by:

Month, Week, Day
Product Category
Location
Sales Trends and Seasonality:

Analyze trends in sales by category, location, and month.
Investigate how sales vary on different days of the week.
Revenue, Marketing Spend, and Tax Analysis:

Measure the monthly revenue, marketing spend (offline and online), and tax percentages.
Analyze how marketing spend impacts revenue generation.
3. Customer Segmentation
Heuristic-based Segmentation (RFM):
Classify customers into Premium, Gold, Silver, and Standard categories based on recency, frequency, and monetary value, and devise strategies for each segment.

Scientific-based Segmentation (K-Means Clustering):
Perform clustering to identify different customer profiles and define tailored strategies for each segment.

4. Customer Lifetime Value (CLV) Prediction
Predict customer lifetime value by categorizing customers into:

Low Value
Medium Value
High Value
Build a classification model to predict the CLV based on historical purchasing behavior.

5. Cross-Selling Analysis
Perform market basket analysis to determine which products are frequently purchased together, allowing for better bundling and marketing strategies.
6. Next Purchase Prediction
Predict the likely next purchase date for each customer (within 0-30 days, 30-60 days, 60-90 days, and 90+ days) using classification models based on customer behavior.
7. Cohort Analysis
Define cohorts based on the first month of purchase and analyze customer behavior within each cohort, identifying the cohort with the highest retention rate.
Features
Comprehensive data analysis: Deep insights into customer behavior, sales trends, marketing spend, and more.
Customer segmentation: Heuristic and scientific approaches to segmenting customers for targeted marketing strategies.
Predictive modeling: Predicting customer lifetime value and next purchase date using machine learning.
Cross-sell recommendations: Market basket analysis to find products that are often purchased together.
Cohort analysis: Detailed cohort analysis to measure customer retention.
Requirements
Python 3.x
Libraries: Pandas, Numpy, Matplotlib, Seaborn, Scikit-learn, Statsmodels, Plotly, and other necessary data science tools.


Run the analysis notebooks to get insights:

License
This project is licensed under the MIT License - see the LICENSE file for details.

Contributing
Feel free to fork the repository, create issues, and submit pull requests. Contributions are welcome!

Contact
For any questions or feedback, feel free to reach out

