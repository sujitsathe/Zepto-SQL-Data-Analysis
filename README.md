# 🛒 Zepto Product Data Analysis (SQL Project)

## 📊 Overview
This project focuses on **exploring and analyzing product data** from **Zepto**, an online grocery delivery platform. Using SQL, it performs **data cleaning, transformation, and insight generation** to understand pricing, discount strategies, product availability, and category-wise revenue.

---

## ⚙️ Tech Stack
- **SQL** (PostgreSQL / MySQL compatible)  
- **Data Source**: Zepto product dataset  

---

---

## 🧩 Key Steps Performed

### 🔹 1. Table Creation
```sql
CREATE TABLE zepto (
  sku_id SERIAL PRIMARY KEY,
  category VARCHAR(120),
  name VARCHAR(150) NOT NULL,
  mrp NUMERIC(8,2),
  discountPercent NUMERIC(5,2),
  availableQuantity INTEGER,
  discountedSellingPrice NUMERIC(8,2),
  weightInGms INTEGER,
  outOfStock BOOLEAN,
  quantity INTEGER
);
🔹 2. Data Cleaning & Validation

Checked for missing values and duplicate products

Removed products with MRP = 0

Converted paise to rupees for accurate pricing

🔹 3. Data Exploration

Found unique categories

Compared in-stock vs out-of-stock products

Analyzed repeated SKUs and pricing anomalies

<img width="968" height="578" alt="image" src="https://github.com/user-attachments/assets/957a8937-7c57-4710-b351-8ae51cb5dda7" />


