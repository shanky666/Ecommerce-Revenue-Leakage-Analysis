📊 E-Commerce Revenue Leakage Analysis
🔎 Project Overview

In many e-commerce businesses, reported sales revenue does not fully translate into realized revenue due to cancellations, undelivered orders, and operational inefficiencies.

This project performs an end-to-end analysis of 100K+ e-commerce transactions to identify revenue leakage and uncover actionable business insights.

🎯 Business Problem

Although order volume is high, actual revenue received is significantly lower than expected.

Key Questions:

What is the gap between Gross Revenue and Net Revenue?

Which order statuses contribute most to revenue leakage?

Which product categories are high-risk?

Where should business intervention be prioritized?

📂 Dataset

Dataset Used: Olist E-Commerce Public Dataset

Files analyzed:

Orders dataset

Order items dataset

Products dataset

Total Records: ~100,000+ transactions

🛠 Tools & Technologies

Python

Pandas (Data Cleaning & Transformation)

Matplotlib (Visualization)

Jupyter Notebook

🔄 Methodology
1️⃣ Data Cleaning

Standardized join keys (order_id, product_id)

Removed formatting inconsistencies

Normalized order_status values

2️⃣ Data Merging

Joined order items with order status

Merged product category information

Ensured accurate relational mapping

3️⃣ Revenue Modeling

Created a delivery-based revenue recognition model:

Gross Revenue = price + freight_value

Earned Revenue = Revenue from delivered orders only

Revenue Leakage = Gross Revenue − Earned Revenue

4️⃣ Analytical Breakdown

Leakage by Order Status

Leakage by Product Category

Leakage Percentage by Category

📈 Key Findings

A measurable gap exists between Gross and Net Revenue.

Canceled and undelivered orders are the primary drivers of revenue leakage.

Certain product categories show disproportionately high leakage percentages.

Leakage is not evenly distributed — targeted operational improvements are possible.

📊 Sample Visualizations
Gross vs Net Revenue

<img width="521" height="306" alt="image" src="https://github.com/user-attachments/assets/723b3ba6-762e-4c7f-90c6-84372496340f" />


Revenue Leakage by Order Status

<img width="649" height="312" alt="image" src="https://github.com/user-attachments/assets/219075d1-3938-4191-9930-16a20d36126f" />


Top 10 Categories by Leakage

<img width="794" height="379" alt="image" src="https://github.com/user-attachments/assets/4fef9fcb-3e80-4ab8-b1ce-cd5724a9a4a8" />


💡 Business Recommendations

Improve delivery fulfillment monitoring.

Reduce cancellation rates through better inventory visibility.

Review high-risk product categories for quality or logistics issues.

Implement operational KPI tracking for leakage reduction.
