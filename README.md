# SQL Retail Analysis: Black Friday & Cyber Week Sales

## Project Overview
This project utilizes SQL to analyze a large retail dataset covering Black Friday, Thanksgiving, and Cyber Monday sales from 2023 to 2025. The goal is to extract actionable business intelligence regarding consumer behavior, discount effectiveness, return rates, and channel mix.

## The Dataset
The dataset contains detailed transaction records, including:
*   Purchase IDs, timestamps, and sales channels (In-store vs. Online).
*   Product details (Brands, Categories, and Types).
*   Financial metrics (List Price, Discount %, Total Revenue).
*   Customer behavior (Ratings, Return reasons, and Coupon usage).

## Business Questions & SQL Techniques Used

This project answers 10 key business questions, demonstrating proficiency in various SQL concepts:

1.  **Purchases, Revenue, and Average Discount by Event Day:** *(Aggregations, GROUP BY)*
2.  **Growth from Year to Year:** *(Date functions, CTEs, Self-Joins)*
3.  **Busiest Hour of Thanksgiving, Black Friday, and Cyber Monday:** *(Window Functions, PARTITION BY)*
4.  **Return Rate by Product Category:** *(Conditional Logic, CASE statements)*
5.  **Do Deeper Discounts Bring More Returns?:** *(Correlation analysis using mathematical operators)*
6.  **Channel Mix on Each Event Day:** *(PIVOT or Conditional Aggregation)*
7.  **The Ten Products with the Most Revenue:** *(ORDER BY, LIMIT)*
8.  **Buy Now, Pay Later (BNPL) Usage & Return Rate:** *(Filtering, Aggregations)*
9.  **Delivery Days by Fulfillment:** *(Date math, EXTRACT/DATEDIFF)*
10. **Coupon Usage & Savings by Event Day:** *(Aggregations, String matching)*

## Key SQL Skills Demonstrated
*   **Advanced Joins:** Merging transactional data with product and category tables.
*   **Window Functions:** Utilizing `RANK()`, `ROW_NUMBER()`, and `PARTITION BY` to identify peak hours and top products without collapsing the dataset.
*   **Data Cleaning in SQL:** Handling NULL values (e.g., `delivery_days` for in-store purchases) and filtering out irrelevant fields (like `return_reason` for non-returned items).
*   **CTEs (Common Table Expressions):** Breaking down complex queries into readable, modular chunks.

## Status
🚧 **Work in Progress:** The SQL scripts (`.sql`) and a Jupyter Notebook containing the queries and their outputs will be uploaded shortly.
