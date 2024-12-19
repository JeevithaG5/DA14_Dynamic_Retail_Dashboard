Here’s an updated and more detailed **README** file that includes sample tables for each dataset:

---

# Dynamic Retail Dashboard in Excel

## Overview
The **Dynamic Retail Dashboard** is a comprehensive and interactive dashboard built in Excel to provide actionable insights into retail operations. It dynamically connects to datasets hosted on GitHub, processes data using Power Query, and visualizes critical metrics with dynamic charts and KPIs. The dashboard is designed to help businesses make data-driven decisions effectively.

---

## Datasets Used

### 1. **Orders Table**
The Orders table contains detailed information about customer orders, including product details, sales, shipping, and profit metrics.

**Sample Data:**
| Order ID       | Returned | Order Date   | Ship Date   | Ship Mode       | Customer Name   | Segment    | Country         | Market | Sales   | Profit   | Discount |
|----------------|----------|--------------|-------------|-----------------|-----------------|------------|-----------------|--------|---------|----------|----------|
| CA-2012-124891 | No       | 31-07-2020   | 31-07-2020  | Same Day        | Rick Hansen     | Consumer   | United States   | US     | 2309.65 | 762.18   | 0        |
| IN-2013-77878  | Yes      | 05-02-2021   | 07-02-2021  | Second Class    | Justin Ritter   | Corporate  | Australia       | APAC   | 3709.40 | -288.77  | 0.1      |
| IN-2013-71249  | No       | 17-10-2021   | 18-10-2021  | First Class     | Craig Reiter    | Consumer   | Australia       | APAC   | 5175.17 | 919.97   | 0.1      |

---

### 2. **Returns Table**
The Returns table tracks orders that have been returned, along with the associated markets.

**Sample Data:**
| Returned | Order ID         | Market         |
|----------|------------------|----------------|
| Yes      | MX-2013-168137   | LATAM          |
| Yes      | US-2011-165316   | LATAM          |
| Yes      | ES-2013-1525878  | EU             |
| Yes      | CA-2013-118311   | United States  |

---

### 3. **People Table**
The People table includes the sales representatives and the regions they are responsible for.

**Sample Data:**
| Person              | Region          |
|---------------------|-----------------|
| Anna Andreadi       | Central         |
| Chuck Magee         | South           |
| Kelly Williams      | East            |
| Matt Collister      | West            |
| Deborah Brumfield   | Africa          |

---

## Problem Statements Solved

### 1. **Key Performance Indicators (KPIs)**
- Metrics calculated:
  - **Total Sales:** Sum of all sales revenue.
  - **Total Profit:** Sum of all profits across orders.
  - **Total Quantity:** Sum of products sold.
  - **Number of Orders:** Count of unique order IDs.
  - **Profit Margin:** Ratio of profit to sales.

**Dynamic Table:**
| KPI                  | Name           | Symbol |
|----------------------|----------------|--------|
| Sum of Sales         | Total Sales    | 💰    |
| Sum of Profit        | Total Profit   | 📈    |
| Sum of Quantity      | Total Quantity | 📦    |
| Count of Order ID    | Total Orders   | 🛒    |
| Sum of Profit Margin | Profitability  | 💹    |

---

### 2. **Sales and Profit Analysis**
- Visualizes sales and profit trends over time.
- Identifies high and low-performing regions.

### 3. **Category-Wise Profit**
- Bar chart comparing profitability across categories such as Furniture, Technology, and Office Supplies.

### 4. **Segment-Wise Sales Share (%)**
- Pie chart visualizing sales share by customer segments (Consumer, Corporate, Home Office).

### 5. **Sales by Country**
- Displays country-wise sales performance using geographic heatmaps.

### 6. **Top 5 Subcategories**
- Identifies subcategories generating the most revenue.

### 7. **Bottom 5 Subcategories**
- Highlights underperforming subcategories.

### 8. **Yearly Sales Trends**
- Line chart displaying sales trends over years.

---

## Steps to Create the Dashboard

### Step 1: Data Connection
- Hosted datasets (Orders, Returns, and People) on GitHub.
- Connected Excel to GitHub for live data updates.

### Step 2: Data Transformation
- Merged tables in Power Query:
  - **Orders + Returns:** To calculate return rates.
  - **Orders + People:** To associate regions with sales reps.
- Created calculated fields such as `Profit Margin` and `Sales Share`.

### Step 3: KPI Calculation
- Formulas used:
  - Total Sales: `=SUM(Sales)`
  - Total Profit: `=SUM(Profit)`
  - Profit Margin: `=SUM(Profit)/SUM(Sales)`
  - Number of Orders: `=COUNTA(Order ID)`

### Step 4: Visualization
- Designed visuals:
  - Bar charts for category analysis.
  - Line charts for trends.
  - Heatmaps for geographical insights.
  - Slicers for interactivity.

### Step 5: Testing and Optimization
- Validated data accuracy.
- Optimized visuals for better interactivity.

---

## Significance
This dashboard empowers retail businesses by:
1. Identifying high and low-performing regions, categories, and subcategories.
2. Providing real-time updates for KPIs.
3. Offering actionable insights into customer behavior and sales trends.

---

## Next Steps for Extension
Future enhancements:
1. **Return Analysis:** Analyze patterns in returns by market.
2. **Top and Bottom Customers:** Identify key contributors to revenue.
3. **Segment Analysis:** Dive deeper into performance by customer segment.
4. **Market Analysis:** Explore market-level sales and profit trends.

---

## Visuals
The repository includes:
- Snapshots of the dashboard for each problem statement.
- Example visuals for KPIs, sales trends, category profits, and more.

---

This README ensures the **Dynamic Retail Dashboard** provides a clear understanding of its features, datasets, problem-solving capabilities, and the process of its creation.
