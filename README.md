# 💎 Jewellery Business Analytics — Power BI Case Study

> Turning jewellery business data into actionable insights using Power BI

---

## 📊 Project Overview

This project is an end-to-end **Power BI Business Analytics case study** designed to demonstrate how raw business data can be transformed into interactive dashboards and meaningful business insights.

The dashboard focuses on key areas of a jewellery business:

- Sales & Revenue
- Products & Categories
- Brands
- Customers
- Instagram Performance
- Marketing Performance

The objective was to build a dashboard that helps business stakeholders understand performance, identify trends, and support data-driven decision making.

---

# 📌 Dashboard Pages

The Power BI dashboard contains six main pages:

### 1. Executive Overview
Provides a high-level summary of business performance.

Key metrics include:

- Total Revenue
- Total Orders
- Total Customers
- Average Order Value
- Instagram Reach
- Engagement

Visualizations include:

- Revenue Trend
- Revenue by Category
- Top Products
- Overall Business KPIs

---

### 2. Instagram Analytics

Analyzes social media performance and audience engagement.

Key metrics include:

- Total Posts
- Total Reach
- Total Engagement
- Average Engagement Rate
- Followers Gained

Analysis includes:

- Engagement by Content Category
- Performance by Media Type
- Reach by Traffic Source
- Top Performing Posts
- Instagram Performance Trends

---

### 3. Product Analytics

Analyzes product and category performance.

Key metrics include:

- Total Revenue
- Total Orders
- Products Sold
- Average Product Price

Analysis includes:

- Revenue by Category
- Orders by Category
- Average Price by Category
- Top Performing Products
- Product Price vs Revenue

---

### 4. Brand Analytics

Analyzes performance across different jewellery brands.

Key metrics include:

- Brand Revenue
- Brand Orders
- Number of Brands
- Average Revenue per Brand

Analysis includes:

- Revenue by Brand
- Orders by Brand
- Revenue Share by Brand
- Brand Revenue Trends
- Brand Performance Summary

---

### 5. Customer Analytics

Provides insights into customer purchasing behaviour.

Key metrics include:

- Total Customers
- Total Orders
- Average Customers
- Repeat Customers

Analysis includes:

- Top Customers by Revenue
- Customer Orders by Category
- New vs Repeat Customers
- Customer Revenue Trends
- Customer Behaviour Insights

---

### 6. Marketing Analytics

Analyzes marketing and Instagram performance.

Key metrics include:

- Total Reach
- Total Engagement
- Average Engagement Rate
- Followers Gained
- Total Posts

Analysis includes:

- Engagement by Content Category
- Reach by Traffic Source
- Engagement Rate by Media Type
- Instagram Performance Over Time
- Top Performing Instagram Posts

---

# 🖼️ Dashboard Preview

## Executive Overview

![Executive Overview]<img width="887" height="499" alt="Jewellery Executive" src="https://github.com/user-attachments/assets/019e5e0b-4dc8-4b73-8cb5-5c6eec532c11" />


---

## Instagram Analytics

![Instagram Analytics]<img width="885" height="497" alt="jecellery Insta" src="https://github.com/user-attachments/assets/c797d611-30c0-42cf-b3ae-20cd3b84fd2e" />


---

## Product Analytics

![Product Analytics]<img width="890" height="498" alt="Jewellery Product" src="https://github.com/user-attachments/assets/d2acf330-518c-41b6-ab3f-7f819965b529" />


---

## Brand Analytics

![Brand Analytics]<img width="890" height="498" alt="Jewellery Brand" src="https://github.com/user-attachments/assets/784a14e3-03c9-427f-9631-a97c231cecb5" />


---

## Customer Analytics

![Customer Analytics]<img width="884" height="497" alt="Jewellery Customer" src="https://github.com/user-attachments/assets/608fc010-f544-4cd4-8c12-e52040cc7869" />


---

## Marketing Analytics

![Marketing Analytics]<img width="884" height="496" alt="Jewellery Marketing" src="https://github.com/user-attachments/assets/11d638e7-7afc-457e-9c72-4810c856dc63" />


---

# 🛠️ Tools & Technologies

The following tools and skills were used in this project:

- Microsoft Power BI
- Power Query
- DAX
- Data Cleaning
- Data Transformation
- Data Modelling
- Data Visualization
- KPI Development
- Business Intelligence
- Business Analytics
- Data Storytelling

---

# 🔍 Business Questions

The dashboard was designed around practical business questions.

## Sales

- What is the total revenue?
- How is revenue changing over time?
- Which jewellery categories generate the most revenue?
- What is the average order value?
- How many orders are being generated?

## Products

- Which products generate the highest revenue?
- Which categories receive the most orders?
- What is the average product price?
- Is there a relationship between product price and revenue?

## Brands

- Which brands generate the most revenue?
- Which brands receive the most orders?
- What percentage of revenue comes from each brand?
- How does brand performance change over time?

## Customers

- How many customers are purchasing?
- Which customers generate the most revenue?
- How many customers are repeat customers?
- What categories do customers purchase?
- How does customer revenue change over time?

## Marketing

- Which content categories generate the most engagement?
- Which media types perform better?
- Which traffic sources generate the most reach?
- Which Instagram posts perform best?
- How does Instagram performance change over time?

---

# 📐 Data Model

The project uses separate business datasets for different analytical areas.

The main datasets include:

### Jewellery / E-commerce Data

Contains information related to:

- Products
- Categories
- Brands
- Prices
- Customers
- Orders
- Purchase events

### Instagram Data

Contains information related to:

- Posts
- Content categories
- Media types
- Reach
- Impressions
- Likes
- Comments
- Shares
- Saves
- Engagement
- Followers gained
- Traffic sources

The datasets are analysed separately where no valid common business key exists.

---

# 📊 Key DAX Measures

## Total Revenue

```DAX
Total Revenue =
SUM(Jewelry[price])

Total Orders =
DISTINCTCOUNT(Jewelry[user_session])

Average Order Value =
DIVIDE(
    [Total Revenue],
    [Total Orders]
)

Total Customers =
DISTINCTCOUNT(Jewelry[user_id])

Products Sold =
COUNTROWS(Jewelry)

Average Product Price =
AVERAGE(Jewelry[price])

Total Posts =
DISTINCTCOUNT(Instagram[post_id])

Total Reach =
SUM(Instagram[reach])

Total Engagement =
SUM(Instagram[likes])
+
SUM(Instagram[comments])
+
SUM(Instagram[shares])
+
SUM(Instagram[saves])

## 🔄 Data Preparation

The data preparation process included:

Importing raw datasets into Power BI
Reviewing column structures
Cleaning and transforming data using Power Query
Checking data types
Creating calculated columns where required
Creating a date table
Building relationships between valid tables
Creating DAX measures
Designing interactive visuals
Testing slicers and dashboard interactions
Formatting the dashboard for business presentation
