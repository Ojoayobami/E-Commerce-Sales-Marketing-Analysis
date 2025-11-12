# 📌 Project Title
🛒 E-Commerce Sales & Marketing Analysis

# 📌 Introduction  
This project analyzes an e-commerce dataset to uncover insights into sales performance, marketing efficiency, and product category trends. The dataset includes total revenue, marketing spend, revenue per marketing spend, and average units sold across different product categories.  

The analysis aims to identify which product categories generate the highest returns, evaluate the effectiveness of marketing investments, and track monthly trends in sales and spend. These insights provide actionable recommendations for optimizing marketing strategies and improving overall business performance.

## 📂 Data Cleaning & Preparation

The dataset was gotten from Kaggle datasets websites.  
During the cleaning phase, several adjustments were made to ensure the dataset was accurate and analysis-ready.

---

### 🧹 Data Cleaning Overview

| Step | Description | Action Taken |
|------|-------------|--------------|
| Removed Duplicates | Ensured each record was unique | Used `Remove Duplicates` (Power Query / Excel) |
| Corrected Data Types | Converted fields to appropriate formats | Revenue, Marketing Spend, Units Sold ➝ Number |
| Fixed Incorrect Date Format | Date column was inconsistent (e.g., `1/1/2023 12:00 AM` vs. `13-01-2023`) and imported as text | Trimmed spaces → Split date/time → Converted to date type → Standardized to `mm/yy/yyyy` |

These steps ensured the dataset was clean, consistent, and ready for visualization and model building.

---

## ⚙️ Calculated Fields & Columns Created

To support advanced analysis of sales and marketing performance, calculated columns were created.

---

### ➕ Calculated Columns

| Column Name | Description |
|-------------|-------------|
| **Revenue** | Calculates total revenue generated per transaction |
| **Discounted_Price** | Shows the price after discount is applied |
| **Revenue per Marketing** | Measures efficiency of marketing spend |
| **Average_Unit_Price** | Shows selling price per unit sold |
| **Discount Rate** | % difference between original price and discounted price |
| **Year** | Extracted from date column to enable yearly trend analysis |
| **Quarter** | Groups dates into Q1, Q2, Q3, Q4 to identify seasonal patterns |

## 🔧 Data Transformation Tools Used

During the data preparation and transformation stage, the following tools were used to clean, format, and prepare the dataset for analysis:

| Tool / Platform | Purpose | Key Actions Performed |
|------------------|----------|------------------------|
| **Power Query (Excel)** | Initial data review and quick cleaning | Removed duplicates, checked column consistency | Changed data types, fixed date formatting, trimmed spaces |
| **Pivot Tables (Excel)** | Data summarization and exploration | Aggregated revenue, units sold, and marketing spend |
| **Microsoft Excel** | Data visualization | Created calculated columns and KPIs |
| **GitHub** | Version control and documentation | Stored cleaned dataset and project documentation |

---

These tools helped streamline data ingestion, cleaning, transformation, and visualization across the entire analysis process.

## 🔍 Exploratory Data Analysis (EDA)

After cleaning and transforming the dataset, an exploratory data analysis was performed to understand sales trends, marketing effectiveness, and revenue distribution across product categories.

### ✅ Key EDA Steps

| Analysis Performed                        | Purpose / Insight Gained |
|-------------------------------------------|---------------------------|
| **Pivot Tables (Excel)**                  | Summarized Revenue, Units Sold, and Marketing Spend across product categories and months. |
| **Trend Analysis (Line Charts)**          | Identified month-to-month changes in revenue and marketing spend. |
| **Category Performance Analysis**         | Compared performance of Home Decor, Fashion, and Electronics using revenue and units sold. |
| **Marketing Efficiency Analysis**         | Calculated Revenue Per Marketing Spend to determine ROI across categories. |
| **Discount Impact Review**                | Compared Discount Rate vs Revenue to observe how discounts affect sales. |

### 📊 Insights Uncovered

- Average units sold per month: **30**
- Total revenue generated: **$15,002,485**
- Product category with highest revenue: **Sports**
- Marketing spend had a measurable impact on revenue, supported by *Revenue Per Marketing Spend* calculated column.

These findings guided visualization and storytelling in the report/dashboard phase.

## 📈 Statistical Analysis

To better understand the relationship between marketing activity, revenue performance, and customer buying behavior, key statistical calculations were applied to the dataset.

### ✅ Statistical Techniques Used

| Technique Applied               | Purpose / Insight |
|--------------------------------|-------------------|
| **Correlation Analysis**       | Measured the relationship between Marketing Spend and Revenue. |
| **Descriptive Statistics**     | Summarized total and average values (Revenue, Units Sold, Marketing Spend). |
| **Revenue per Marketing (RPM)**| Evaluated marketing efficiency. |
| **Category & Customer Contribution Analysis** | Identified the highest revenue category and customer segment. |

### 📊 Findings from Statistical Analysis

| Metric / Result                                                   | Insight |
|------------------------------------------------------------------|---------|
| **Strong positive correlation** between Marketing Spend and Revenue | Higher marketing spend generally led to higher revenue. |
| **Sport category generated the highest total revenue**              | Sport products produced the largest share of sales. |
| **Electronics had the highest marketing spend**                    | However, it did *not* generate the highest revenue — indicating lower marketing efficiency. |
| **Occasional customers contributed the most to total revenue (35%)** | Irregular/one-time buyers impact sales more than regular or premium buyers. |
| **Units sold increased with higher discount price**                | Discounts encouraged purchases, especially in Electronics & Toys. |
| **Revenue per Marketing Spend (RPM) = $6,992**                     | For every $1 spent on marketing, the business generated **$6.99** in revenue. |

---

These statistical results validate the impact of marketing spend on revenue and highlight where the business should focus its efforts for maximum ROI.

## 🧠 INSIGHTS & RECOMMENDATIONS

---

## 📌 Key Insights

### 1. Total Business Performance

| Metric | Value |
|--------|-------|
| Total Revenue | **$15,002,485** 💰 |
| Total Marketing Spend | $4,912,830 📊 |
| Revenue per Marketing Spend (ROI) | **$6,992** 🚀 |
| Average Units Sold | 30 units per product 📦 |

> 💡 For every $1 spent on marketing, the business generates **$3.05 in revenue** ($15M / $4.9M).

---

### 2. Product Category Performance

| Category | Marketing Spend | Revenue | Efficiency (Revenue per $1 Marketing) |
|----------|----------------|---------|--------------------------------------|
| Home Decor | $938,726 | $2,779,860 | $2.96 |
| Fashion | $920,955 | $2,968,174 | **$3.22** ⭐ |
| Electronics | $1,064,354 | $3,022,450 | $2.84 |
| Toys | $1,010,548 | $3,030,592 | $3.00 |
| Sports | $978,248 | $3,201,408 | **💥 $3.27 (Best ROI)** |

> ⚡ **Sports & Fashion** generate the highest revenue return per $1 spent on marketing.

---

### 3. Discount vs Demand (Category Level)

| Category | Discounted Revenue | Units Sold |
|----------|-----------------|------------|
| Sports | $103,438 | 6,125 |
| Electronics | $97,303 | 6,210 **🏆 Highest Units Sold** |
| Toys | $96,062 | 6,003 |

> 💡 Discounting increases unit sales. **Electronics** responds best to discount-driven promotions.

---

### 4. Customer Segments

| Segment | Revenue Share | Discounted Spend | Units Sold |
|---------|---------------|-----------------|------------|
| Occasional | 35% (Top segment) | $169,730 | 9,842 |
| Regular | 34% | $163,164 | 10,222 **🏅 Highest Units Sold** |
| Premium | 31% | $147,428 | 9,567 |

> 💡 Occasional buyers generate the most revenue, but **Regular buyers show the highest purchase volume**.

---

### 5. Yearly Trends

| Year | Revenue | Marketing Spend |
|------|---------|----------------|
| 2024 | **$5,552,401** 📈 | $1,808,556 |
| 2023 | $5,475,563 | $1,802,026 |
| 2025 | $3,974,520 | $1,302,249 |

> 📊 2024 is the best performing year for both revenue and marketing ROI.

---

### 6. Monthly Trend Analysis

- **July** recorded the highest revenue: $1,464,739 💰 despite lower marketing spend.
- **November & October** show a revenue drop — likely **post-season decline** 📉.
- Marketing spend is high early in the year, but returns peak mid-year, showing **improved efficiency** ⚡.

---

## ✅ Recommendations

1. **Invest more marketing budget into Sports, Fashion, and Toys**
   - These categories deliver the highest ROI and revenue growth potential.
   - 🌟 Expected outcome: Higher revenue without increasing overall ad spend.

2. **Activate targeted campaigns for Regular & Premium segments**
   - Regular customers buy the most units → ideal for upselling bundles.
   - Premium segment prefers value → less discount, more exclusivity.
   - 🎯 Offer exclusive early-access or loyalty bonuses.

3. **Push seasonal & discount campaigns during months with high responsiveness**
   - Increase budget during **June–August (peak buying)** 📅.
   - Reduce spend in **October–November** (low conversion period) 📉.
   - ⏳ Timing marketing around seasonal demand will maximize impact.

4. **Reduce blanket discounting**
   - Use discounts strategically on:
     - **Electronics** (highest response to discounts) 💡
     - **Sports** during peak season (highest ROI) 💥
   - 💡 Strategic discounting improves volume without hurting profit.

5. **Create bundles for underperforming categories (Home Decor)**
   - Home Decor has the lowest ROI.
   - 📦 Bundle Home Decor with high-performing categories like Fashion or Toys.

---

### 🚀 Final Strategic Focus

> Prioritize **high ROI categories**, target **Regular & Premium customers** with personalized offers, and run **seasonal marketing during peak months** to improve total revenue without overspending.

## Main Dashboard

![Business Dashboard.E-Commerce Dashboard.png
