# TASK-3
# SQL SELECT Queries (E-commerce Example)

## ✅ What this task is about

In this task, I learned how to **get data** from a database using SQL.  
I used simple `SELECT` queries to show data from two tables: **Customers** and **Orders**.

## 📚 What I learned

- How to show **all columns** or **only specific columns**
- How to filter data using **WHERE**, **AND**, **OR**
- How to search using **LIKE**
- How to get data in a **range** using **BETWEEN**
- How to sort results using **ORDER BY**
- How to show only a few rows using **LIMIT**

## 🗂️ Tables I used

### 🧍 Customers table
Stores customer details:
- ID, Name, Email, Phone, City

### 📦 Orders table
Stores order details:
- Order ID, Customer ID, Order Date, Amount, Status

## 🔑 Important concepts

- **Filtering** → Showing only the data I need (like customers from Mumbai)
- **Projection** → Showing only specific columns (like name and city)
- **Sorting** → Showing data in order (like highest to lowest amount)
- **Limiting** → Showing only top rows (like top 2 orders)

## 💻 Tool I used

- **DB Browser for SQLite**

## 📁 Files in this task

- `ecommerce_select_queries.sql` → This file has all the SQL queries I wrote
- `README.md` → This file (explains what I did)

## 🧪 Some examples of my queries

```sql
-- Show all customers
SELECT * FROM Customers;

-- Show customer names and cities
SELECT name, city FROM Customers;

-- Orders between ₹500 and ₹1500
SELECT * FROM Orders WHERE total_amount BETWEEN 500 AND 1500;

-- Emails that contain the word 'example'
SELECT * FROM Customers WHERE email LIKE '%example%';

-- Orders sorted from high to low amount
SELECT * FROM Orders ORDER BY total_amount DESC;

