# MySQL Project: E-Commerce Customer Churn Analysis

## Project Overview
This SQL project focuses on analyzing customer churn behavior in an e-commerce business. The dataset contains transaction and behavioral attributes including purchase frequency, app usage, payment methods, satisfaction score, and churn status.

## Project Structure
- MySQL Project.sql: Main SQL script containing table creation and data insertion.
- README.md: Project documentation.

## Steps Performed in SQL

### 1. Create Database
```
CREATE DATABASE ecomm;
USE ecomm;
```

### 2. Create Table
A table `customer_churn` was created with fields such as CustomerID, Churn, Tenure, PreferredLoginDevice, CityTier, SatisfactionScore, CouponUsed, OrderCount, and CashbackAmount.

### 3. Insert Data
500+ customer records were inserted to simulate real-world e-commerce customer behavior.

### 4. Basic Data Retrieval
```
SELECT * FROM customer_churn;
```

## Example Analysis Queries

### 1. Churn Distribution
```
SELECT Churn, COUNT(*) 
FROM customer_churn
GROUP BY Churn;
```

### 2. Average Tenure by Churn
```
SELECT Churn, AVG(Tenure)
FROM customer_churn
GROUP BY Churn;
```

### 3. Preferred Payment Mode
```
SELECT PreferredPaymentMode, COUNT(*)
FROM customer_churn
GROUP BY PreferredPaymentMode
ORDER BY COUNT(*) DESC;
```

## Conclusion
This MySQL project demonstrates table creation, data insertion, and customer churn analysis using SQL. It serves as a strong portfolio project for Data Analyst, BI, and SQL Developer roles.
