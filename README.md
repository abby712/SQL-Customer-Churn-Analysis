# MySQL Project: E-Commerce Customer Churn Analysis

## 📌 Project Overview
This SQL project focuses on analyzing customer churn behavior in an e-commerce business.  
The dataset includes customer details such as purchase behavior, login device, payment preferences, app usage, and churn status.  
The analysis helps identify churn patterns and business improvement opportunities.

---

## 📁 Project Files

### 👉 **[Open MySQL Project.sql](./MySQL%20Project.sql)**
Click the link above to open or download the SQL script without formatting issues.

### 📥 Download Button  
[![Download SQL](https://img.shields.io/badge/Download-SQL%20File-blue)](./MySQL%20Project.sql)

---

## 🛠️ How to Open and Run the SQL File

### 🔹 **Option 1: MySQL Workbench**
1. Open **MySQL Workbench**
2. Go to **File → Open SQL Script**
3. Select **MySQL Project.sql**
4. Click **Run** (Lightning icon)

### 🔹 **Option 2: phpMyAdmin (XAMPP, WAMP, Laragon, etc.)**
1. Open **phpMyAdmin**
2. Select the database (or create one)
3. Click **Import**
4. Upload **MySQL Project.sql**
5. Click **Go**

### 🔹 **Option 3: MySQL Command Line**
```bash
mysql -u root -p < "MySQL Project.sql"
```

---

## 📊 Steps Performed in SQL

### 1️⃣ Create Database
```sql
CREATE DATABASE ecomm;
USE ecomm;
```

### 2️⃣ Create Table  
Created `customer_churn` table with attributes such as:
- CustomerID  
- Tenure  
- Churn  
- PreferredLoginDevice  
- SatisfactionScore  
- OrderCount  
- CashbackAmount  
… and more.

### 3️⃣ Insert Data  
Inserted **500+ records** simulating real-world customer activity.

### 4️⃣ Basic Retrieval
```sql
SELECT * FROM customer_churn;
```

---

## 📈 Example Analysis Queries

### 🔸 Churn Distribution
```sql
SELECT Churn, COUNT(*)
FROM customer_churn
GROUP BY Churn;
```

### 🔸 Average Tenure by Churn
```sql
SELECT Churn, AVG(Tenure)
FROM customer_churn
GROUP BY Churn;
```

### 🔸 Most Preferred Payment Mode
```sql
SELECT PreferredPaymentMode, COUNT(*)
FROM customer_churn
GROUP BY PreferredPaymentMode
ORDER BY COUNT(*) DESC;
```

---

## ✅ Conclusion
This project demonstrates:
- SQL table creation  
- Data insertion  
- Exploratory churn analysis  
- Portfolio-ready SQL skills  

Useful for roles like **Data Analyst, SQL Developer, and BI Analyst**.
