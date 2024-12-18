
# Excel Coffee Sales Dashboard
![Excel project](https://github.com/user-attachments/assets/5bf2b737-9089-46c2-ad81-2796f8cb6344)

The Coffee Sales Dashboard analyzes sales data spanning from **2019 to 2022** to uncover trends, insights, and performance drivers across key dimensions, including roast type, product size, geographic distribution, and customer loyalty. This interactive dashboard empowers stakeholders to explore sales performance visually and dynamically filter data. The primary focus is to:
- Identify **sales trends** over time.
- Pinpoint **top-performing regions** and customer segments.
- Evaluate roast types, size preferences, and the impact of loyalty programs.

The dashboard provides decision-makers with actionable insights to optimize sales, target growth opportunities, and improve customer retention.

## **Executive Summary**
Between **2019 and 2022**, coffee sales demonstrated fluctuating trends driven by factors such as seasonality, roast type preferences, and country-specific performance. Key findings include:
1. **United States** emerged as the top-performing country with sales of **RM35,639**, significantly outperforming other regions like Ireland (**RM6,697**) and the United Kingdom (**RM2,799**).
2. Among the roast types:
   - **Arabica** dominated sales, particularly in the first half of each year.
   - Other varieties, such as **Excelsa** and **Robusta**, experienced lower but consistent sales contributions.
3. The **top 5 customers** generated revenues ranging between **RM278** to **RM317**, led by **Allis Wilmore**.
---
## **Insights Deep-Dive**

### **1. Total Sales Over Time**
![Picture1](https://github.com/user-attachments/assets/c3671a2d-40e3-40e5-8677-d7def847b13c)

- Sales showed **seasonal peaks** each year, particularly around **April–May** and **September–October**, likely influenced by holidays, promotions, or seasonal demand.
- There were noticeable dips in sales across all years, particularly around **February and August**, signaling potential off-peak periods.

### **2. Sales by Country**
![Picture2](https://github.com/user-attachments/assets/8fd45ac4-05c4-495e-b2a0-942201f0d769)

- **United States** contributed over 80% of total sales, underscoring it as the dominant market.
- **Ireland** and **United Kingdom** showed growth potential but remain underperforming compared to the US.
- Geographic sales disparity suggests an opportunity to expand marketing efforts in smaller regions.

### **3. Product and Customer Preferences**
![Picture3](https://github.com/user-attachments/assets/aaa67446-9609-4b32-ba76-a18a7d11f375)

- **Arabica** led sales compared to Excelsa, Liberica, and Robusta, highlighting customer preference for high-quality coffee.
- The **top 5 customers** contributed significantly to overall sales, with revenue per customer ranging from **RM278 to RM317**.

### **4. Loyalty Programs**
- **Loyalty card holders**' average spending was lower than that of non-card holders. This suggests that opportunities exist to incentivize higher spending among cardholders.
---

## **Recommendations**

1. **Geographic Expansion**
   - Focus marketing efforts in regions like **Ireland** and the **United Kingdom** to drive sales growth.
   - Introduce targeted campaigns to leverage untapped markets while maintaining stronghold in the United States.

2. **Boost Seasonal Sales**
   - Capitalize on peak periods (April–May and September–October) through promotions, bundled offers, and discounts to maximize revenue.
   - Introduce loyalty-based incentives during low-sales months (February and August) to improve demand consistency.

3. **Product and Roast Optimization**
   - Prioritize the production and promotion of **Arabica** coffee, given its dominant market share and customer preference.

4. **Enhance Loyalty Programs**
   - Expand loyalty card initiatives to attract non-cardholders by offering rewards such as **discounts, referral bonuses, or free samples**.
   - Personalize promotions for loyal customers to maintain long-term relationships and encourage higher spending.

5. **Target High-Value Customers**
   - Focus on retaining top customers, like **Allis Wilmore**, through exclusive offers or personalized communication.
   - Develop strategies to identify and nurture high-potential customers, ensuring they contribute more to overall sales.

---



## **Excel**
The dataset was prepared using **XLOOKUP** to retrieve Customer Name, Email, and Country based on Customer ID, replacing missing Email values with blanks for consistency. **INDEX MATCH** dynamically pulled product details like Coffee Type, Roast Type, Size, and Unit Price using Product IDs. Abbreviations in Coffee Types (e.g., "ROB" → "Robusta") and Roast Types (e.g., "M" → "Medium") were expanded with **Multiple IF Functions**. **Date Formatting** standardized Order Dates to a user-friendly format (e.g., "05-Sep-2019"), and duplicates were removed using **Remove Duplicates**. The raw data was structured into a table format with **Convert Range to Table** for improved management.

Total Sales were calculated by multiplying Unit Price with Quantity Sold. **Pivot Tables** summarized sales trends, grouping dates by Year/Month and analyzing data across Coffee Types and Sales. Tables were formatted to remove decimals and apply number formatting. The Pivot Table data source was refreshed using table references, with a "Loyalty Card" column auto-populated via XLOOKUP. **Slicers** and **Timelines** were added for interactive filtering.

For visual insights, the **Sales by Country** bar chart was customized by sorting countries based on sales and enhancing the layout with colors and labels. A **Top 5 Customers** chart was created by filtering top sales contributors. The final **dashboard** was assembled by integrating charts, slicers, and timelines, ensuring a clean layout with consistent filtering and a polished, user-friendly presentation.
To retrieve Customer Name, Email, and Country based on Customer ID, XLOOKUP was utilized. Missing values in the Email field were replaced with blank spaces instead of zeros to ensure data consistency.
