# E-Commerce Customer Churn Analysis

## Project Overview

This project focuses on analyzing customer churn in an e-commerce dataset using MySQL.

The analysis includes data cleaning, data transformation, exploratory data analysis (EDA), customer churn analysis, distance categorization, and customer return analysis.

## Tools Used

- MySQL
- SQL
- GitHub

## Dataset

The project uses an E-Commerce Customer Churn dataset containing customer information such as:

- Customer demographics
- Tenure
- Preferred login device
- Preferred order category
- Preferred payment mode
- City tier
- Warehouse-to-home distance
- Hours spent on app
- Order count
- Satisfaction score
- Cashback amount
- Churn status
- Complaint information

## Data Cleaning

The following data cleaning operations were performed:

- Missing values were imputed using mean values for numerical columns.
- Missing values were imputed using mode values for categorical/count columns.
- Outlier records where `WarehouseToHome > 100` were removed.
- Data inconsistencies were corrected in login device, order category, and payment mode columns.

## Data Transformation

The following transformations were performed:

- Renamed `PreferedOrderCat` to `PreferredOrderCat`.
- Renamed `HourSpendOnApp` to `HoursSpentOnApp`.
- Created `ComplaintReceived` based on complaint information.
- Created `ChurnStatus` to classify customers as `Churned` or `Active`.
- Created distance categories based on `WarehouseToHome`.
- Removed the original `Churn` and `Complain` columns after transformation.

## Exploratory Data Analysis

The analysis includes:

- Count of churned and active customers
- Average tenure and total cashback of churned customers
- Percentage of churned customers who complained
- Churn analysis by city tier and preferred order category
- Most preferred payment mode among active customers
- Order amount hike analysis
- Average devices used by UPI users
- Customer distribution by city tier
- Coupon usage by gender
- Customer count and maximum app usage by order category
- Order count analysis for credit-card users
- Average satisfaction among customers who complained
- Preferred order categories among customers using more than five coupons
- Top categories based on average cashback
- Payment mode analysis based on tenure and order count
- Distance category analysis
- Analysis of high-order-count customers based on marital status and city tier

## Customer Returns Analysis

A separate `customer_returns` table was created containing:

- Return ID
- Customer ID
- Return date
- Refund amount

Return details were joined with customer information to identify churned customers who had also submitted complaints.

## Project Files

- `ecommerce_customer_churn_analysis.sql` - Complete MySQL queries used for the analysis
- `README.md` - Project documentation

## Key Skills Demonstrated

- SQL
- MySQL
- Data Cleaning
- Data Transformation
- Exploratory Data Analysis
- Aggregation and Grouping
- Joins
- CASE Statements
- Missing Value Handling
- Customer Churn Analysis
- Data Segmentation

## Conclusion

This project demonstrates the use of MySQL for cleaning, transforming, and analyzing e-commerce customer data to understand customer churn patterns and related customer behavior.
