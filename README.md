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

 ## Key Business Insights & Analysis
 1. Event Day & Year-over-Year Momentum
* Black Friday is the clear wave: It pulls the highest volume (106,314 purchases) and top revenue ($17,506,703.83), paired with the steepest average discount (38.42%), followed by Cyber Monday ($14,493,895.30, 33.44% avg discount) and Black Friday weekend ($13,021,902.46, 25.92% avg discount).

* Early November punches above its discount weight: It ranks 4th in revenue ($12,138,206.84) despite a relatively low 10.94% average discount, meaning buyers are already shopping early without needing massive markdowns.

* Steady YoY growth: Total revenue climbed 11.55% in 2024 ($26,373,285.30 vs. $23,641,996.74 in 2023) and 11.44% in 2025 ($29,389,579.67), showing consistent annual expansion rather than a one-off spike.

 2. Peak Traffic Windows & Timing
* Morning rush on Black Friday vs. evening everywhere else: Black Friday peaks at hour 7 (7,314 orders), while almost every other window—Cyber Monday (5,475), Black Friday weekend (5,246), Early November (4,041), Cyber Week (3,440), and Thanksgiving week (3,066)—peaks at hour 19 (7 PM), and Thanksgiving peaks at hour 20 (8 PM, 3,507 orders).

* Takeaway for campaigns: Schedule early-bird/doorbuster pushes right before 7 AM on Black Friday, and lean into evening promos around 7–8 PM across the rest of the holiday stretch.

  3. Returns, Discounts & High-Ticket Products
* Apparel leads category returns by a wide margin: Apparel sits at a 41.27% return rate (30,111 returns out of 72,954 orders), ahead of Jewelry (28.09%) and Electronics (18.65%), whereas Books (9.30%) and Beauty (11.52%) have the lowest return rates.

* Deeper discounts track with higher return rates: Orders with 50%+ Off see a 42.75% return rate (5,814 of 13,599), compared to 22.96% for 21–50% Off, 14.56% for 1–20% Off, and 8.57% for No Discount—classic sign of impulse/size-guess buying on steep promos.

* Laptops and 4K Smart TVs drive top product revenue: The top 8 revenue products are all Laptops and 4K Smart TVs (led by Orbitek Laptop at $3,468,178.19 and Voltrix Laptop at $3,385,522.94), followed by Lumora Tablet and Voltrix Tablet.

4. Fulfillment, Coupons & Data Watchouts
* Fast fulfillment vs. standard shipping lag: Pick up in store averages 0.5 days, Express shipping 1.5 days, and Free 2-day shipping 2.5 days, while Standard shipping stretches to 6.37 days.

* Coupons concentrate on peak days: Black Friday (27,681 orders, $469,759.48 savings) and Cyber Monday (21,236 orders, $391,327.72 savings) carry the heaviest coupon redemption and savings totals.
