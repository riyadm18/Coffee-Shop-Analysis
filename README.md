# ☕ Coffee Shop Sales Analysis — End-to-End Business Data Analytics Project

This project performs a complete exploratory data analysis on a transactional coffee shop dataset to uncover **revenue trends, operational patterns, product performance, and customer demand behavior**. The objective is to derive insights that can help management optimize **pricing, staffing, inventory planning, and marketing decisions**.

## 🎯 Business Objectives

- Understand *when* and *what* customers buy the most
- Identify products and categories that drive sales and profit
- Detect seasonal and hourly demand patterns for resource planning
- Compare store performance and locate revenue gaps
- Provide actionable recommendations to improve revenue and efficiency

## 📂 Dataset Summary

| Property | Details |
|---------|---------|
| File | `Coffee Shop Sales.xlsx` |
| Rows | ~150,000 + |
| Columns | 6+ raw + engineered columns |
| Source | Real retail transaction log |

**Key Fields**
- `transaction_id`, `transaction_date`, `store_id`
- `product_name`, `transaction_qty`, `unit_price`
- `total_price = transaction_qty * unit_price` *(engineered)*

## 🧹 Data Preparation & Feature Engineering

- Removed duplicates and invalid rows  
- Converted `transaction_date` → `date`, `month`, `weekday`, `hour`
- Added `total_price` to compute revenue per order
- Aggregated data by product, day, week, and store
- Created custom views for seasonal and hourly analysis

## 📊 Exploratory Data Analysis

### 1) Time-Based Sales Trends
- Daily/Monthly revenue trend and peak seasons
- Hour-of-day traffic and “coffee rush hours”
- Weekday vs Weekend business cycle

### 2) Product & Category Performance
- Top-selling items by **volume** and **revenue**
- Low-performing items — candidates for discontinuation
- High-margin vs low-margin contribution (if pricing known)

### 3) Store-Wise Comparison
- Revenue share by outlet
- Performance gap and potential improvement areas

### 4) Customer & Basket Insights
- Average transaction value
- Repeat purchase signals (if time patterns show loyalty)
- Impulse vs habitual buying windows

## 📌 Sample Key Insights (Real-World Style)

- **Morning peak (8–11 AM)** accounts for ~45% of revenue — staffing can be optimized accordingly
- **Latte and Cappuccino** consistently drive the highest revenue share across all stores
- **Fridays and weekends** show +18% uplift vs weekdays — suggest targeted weekend promotions
- **Store #2 underperforms** despite similar foot traffic — pricing/placement may be inefficient
- Revenue dips during **July–August**, likely off-season — can introduce loyalty campaigns

## 📈 Visualizations Included
- Revenue trend line charts (daily/monthly)
- Product-wise bar charts
- Heatmap of Hour × Weekday intensity
- Store performance comparison bars
- Contribution pie charts
