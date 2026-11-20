# Customer Behaviour Analysis | Python, SQL, Power BI

## Problem Statement
Understanding what customers buy is only part of the picture. Retail businesses also need to understand why they buy, what influences their spending, and what brings them back.

A leading retail company wants to use its customer shopping data to uncover these patterns, understand differences in purchasing behaviour across customer segments, and identify opportunities to improve sales and build lasting customer loyalty.

Key Business Question: **What drives customer purchasing decisions and repeat purchases, and how can these insights help the company make smarter marketing, pricing and product decisions?**

---

## Dashboard Preview
## 👉 **Live Dashboard:** [View Power BI Dashboard](https://app.fabric.microsoft.com/view?r=eyJrIjoiYzJjZjBkZWQtYTU5My00MjY2LTliYTAtMzY5YWJkOTE2OTY3IiwidCI6ImE1ZmI3ZjgwLTIwNTEtNGE5Ny05YjEyLTZhYjIyMmQyYmQ1NSJ9)

---

## Dashboard Screenshots

Bookmark 1: Customer Performance
<img width="1189" height="646" alt="image" src="https://github.com/user-attachments/assets/0f97bc5b-0846-46f9-9e55-412d74de149d" />

Bookmark 2: Customer Behaviour
<img width="1188" height="643" alt="image" src="https://github.com/user-attachments/assets/5e559b78-d974-46e5-918e-497e442981f7" />

---

## Key Business Insights

- **Customer Loyalty:** Around 60% of customers fall into the loyal segment, while only 11% are new customers.
- **Subscription Opportunity:** Only around 30% of repeat buyers with more than 5 previous purchases have a subscription, that shows there is a scope to improve subscription adoption.
- **Discount Behaviour:** Customers using discounts show a higher average purchase value than those who didn't, that shows there is an association between discount usage and spending.
- **Category Performance:** Electronics generates the highest overall revenue among product categories.
- **Customer Segments:** Customers aged 46–60 contribute the highest revenue, while the 60+ segment records the highest average purchase value.

---

## Tools and Technologies

- **Python:** Pandas, NumPy
- **SQL (MySQL):** Aggregations, subqueries, CTE's and window functions
- **Power BI:** DAX, Bookmarks

---

## Analytical Approach

### 1. Data Cleaning and EDA (**Python**): 
- **Missing Values**: Identified 2,075 missing entries across four columns: Purchase Amount (556), Size (370), Review Rating (601) and Previous Purchases (548). Investigated the missing values and handled them to prepare the dataset for analysis.
- **Duplicates**: Found out 50 duplicate rows. Dropped the duplicate rows keeping the first instance.
- **Incorrect Category Mapping**: Found products assigned to incorrect categories, such as Shirts and Shoes appearing under unrelated categories. Created a custom dictionary mapping to assign each product to its correct category.
- **Data Validation & EDA**: Examined data types, statistical summaries and unique values to understand the dataset and identify inconsistencies before proceeding with business analysis.

### 2. Business Analysis (**SQL**):
- Answered 12 business-driven questions to examine revenue, discounts, customer segments, subscriptions, product ratings and purchasing preferences.
- **Revenue Analysis**: Compared revenue and average purchase value across product categories and customer demographics using aggregate functions and GROUP BY.
- **Discount Analysis**: Examined discount usage patterns and identified customers who spent above the overall average despite using discounts.
- **Product & Shipping Analysis**: Evaluated product ratings, discount frequency and revenue across shipping methods.
- **Customer Segmentation**: Classified customers as New, Returning and Loyal using CASE and UNION ALL; also compared subscription patterns among repeat buyers.
- **Advanced SQL**: Used subqueries, CTEs and window functions (RANK()) to identify above-average spenders and top-selling products within each category.

### 3. Data Visualization (**Power BI**): 
- **Dashboard Structure:** Created two interactive views using bookmarks and page navigation to separate Customer Performance and Customer Behaviour analysis.
- **KPI Tracking:** Developed DAX measures and KPI cards to track total customers, distinct products, average rating, total spend, average spend and subscription rate.
- **Customer Performance Analysis:** Used charts to analyse revenue by customer segment, category-wise spending, subscription patterns, purchase frequency, discount usage and top-performing locations.
- **Customer Behaviour Analysis:** Explored gender-based category preferences, seasonal spending patterns, shipping methods, age-wise spending and category preferences across customer segments.

---

## Conclusion

The analysis shows that customer purchasing behaviour varies across product categories, customer segments and engagement patterns. Electronics and Accessories together account for nearly 80% of total spending, while subscribers show higher average spending than non-subscribers.

Although loyal customers form a substantial part of the customer base, subscription adoption remains an opportunity for improvement. Differences in discount usage and spending across customer segments also highlight the need for more targeted customer strategies.

These insights can help the business make better-informed decisions around product planning, customer targeting, promotional strategies and retention.
