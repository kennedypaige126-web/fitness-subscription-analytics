# fitness-subscription-analytics

Project Overview

This project analyzes customer subscription behavior for FitnessHub, a subscription-based fitness platform offering personalized workout plans, nutrition coaching, and on-demand fitness classes.

The objective of this analysis is to understand customer retention patterns, forecast future subscription revenue, and evaluate how long it takes customer cohorts to recover their acquisition costs. The findings help leadership assess the sustainability of the company's growth strategy and identify opportunities to improve long-term customer value.

Business Questions

This project answers the following business questions:

After how many months do customers typically cancel their subscriptions?
What is the expected subscription revenue over the next 12 months?
How long does it take for customer cohorts to recover their customer acquisition cost (CAC)?
Dataset

The analysis uses the Fitness_Subscriptions_Dataset.xlsx workbook containing two worksheets:

Customers

Contains customer acquisition and subscription information.

Key fields:

Customer_ID
Subscription_Plan
Country
Acquisition_Channel
CAC
Transactions

Contains customer purchases and subscription revenue information.

Key fields:

Transaction_ID
Customer_ID
Transaction_Date
Revenue
Transaction_Type
Product
Tools and Technologies
Power BI Desktop
DAX
Excel
GitHub

Key Power BI techniques used:

Cohort Analysis
Revenue Forecasting
Time Intelligence
Customer Lifetime Value (LTV) Analysis
Customer Acquisition Cost (CAC) Analysis
Data Model

The report uses a star schema data model consisting of:

customers
transactions
dim_date

Relationships:

customers[Customer_ID] → transactions[Customer_ID]
dim_date[Date] → transactions[Transaction_Date]
Customer Cohort Analysis

The cohort analysis groups customers based on the month they began their subscription and tracks retention over time.

Key Finding

Customers typically begin cancelling their subscriptions after approximately [X] months, with the largest decline in retention occurring between Month [X] and Month [X].

This indicates that the first few months of the customer lifecycle are the most critical period for retention initiatives.

Revenue Forecast

Monthly subscription revenue was analyzed using Power BI's built-in forecasting functionality with a 12-month forecast horizon and 95% confidence interval.

Key Finding

The forecast predicts that subscription revenue will [increase/remain stable/decrease] over the next 12 months.

The forecast [does/does not] show evidence of seasonality, suggesting that customer purchasing behavior is [consistent throughout the year/influenced by seasonal patterns].

CAC vs. LTV Analysis

Customer Lifetime Value (LTV) was compared against Customer Acquisition Cost (CAC) to determine profitability timelines for customer cohorts.

Key Findings
The 2024 cohort reached CAC break-even after approximately [X] months.
The 2025 cohort reached CAC break-even after approximately [X] months.

The comparison highlights differences in acquisition efficiency and customer monetization between cohorts.

Business Recommendations
Focus retention efforts during the first few months after signup, when churn risk is highest.
Continue investing in acquisition channels that generate customers with shorter CAC payback periods.
Monitor seasonal revenue patterns to improve marketing and capacity planning.
Track cohort performance regularly to identify changes in customer behavior over time.
