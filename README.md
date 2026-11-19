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

## Results
1.  **Purchases, Revenue, and Average Discount by Event Day:**
   <img width="537" height="206" alt="image" src="https://github.com/user-attachments/assets/b7332bfb-ec5a-4693-9bda-36c0783c3ed2" />
   
2.  **Growth from Year to Year:** 
   <img width="468" height="103" alt="image" src="https://github.com/user-attachments/assets/f252d522-7543-4f06-8b66-3b9988c4873a" />

3.  **Busiest Hour of Thanksgiving, Black Friday, and Cyber Monday:**
   
     <img width="354" height="198" alt="image" src="https://github.com/user-attachments/assets/ab2b80e2-e1fe-4bd6-92ea-02a1d80a7a55" />

5.  **Return Rate by Product Category:**
   
    <img width="433" height="282" alt="image" src="https://github.com/user-attachments/assets/11d87aac-9c53-46a9-a3a2-1b90646026cd" />
    
6.  **Do Deeper Discounts Bring More Returns?:**
    
   <img width="384" height="139" alt="image" src="https://github.com/user-attachments/assets/0d71d9f7-3293-488f-8a89-b8b58351e7e9" />

6.  **Channel Mix on Each Event Day:**

   <img width="455" height="203" alt="image" src="https://github.com/user-attachments/assets/0899bda5-887a-4e78-8893-0aac301e093e" />

7.  **The Ten Products with the Most Revenue:**
   
    <img width="273" height="281" alt="image" src="https://github.com/user-attachments/assets/a523750f-715b-457d-8d44-6dffff05b87c" />
    
8.  **Buy Now, Pay Later (BNPL) Usage & Return Rate:**
   
    <img width="327" height="64" alt="image" src="https://github.com/user-attachments/assets/c3d637ee-d212-4b0f-a4c9-eb0a3fcd8faf" />

9.  **Delivery Days by Fulfillment:**
   
    <img width="283" height="118" alt="image" src="https://github.com/user-attachments/assets/75e660c2-ad35-470a-a911-d5025656a364" />

10. **Coupon Usage & Savings by Event Day:**
    
    <img width="437" height="201" alt="image" src="https://github.com/user-attachments/assets/33f4ba01-8573-4d0f-99c2-0d7832f78750" />
