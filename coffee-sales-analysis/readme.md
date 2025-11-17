{\rtf1\ansi\ansicpg1252\cocoartf2867
\cocoatextscaling0\cocoaplatform0{\fonttbl\f0\fswiss\fcharset0 Helvetica;}
{\colortbl;\red255\green255\blue255;}
{\*\expandedcolortbl;;}
\paperw11900\paperh16840\margl1440\margr1440\vieww34360\viewh18680\viewkind0
\pard\tx720\tx1440\tx2160\tx2880\tx3600\tx4320\tx5040\tx5760\tx6480\tx7200\tx7920\tx8640\pardirnatural\partightenfactor0

\f0\fs24 \cf0 # Coffee Shop Sales Analysis (Jan\'96Jun 2023)\
\
## Dataset Description\
\
The dataset used in this analysis is sourced from [Kaggle: Maven Roasters Coffee Shop Sales & Revenue Dataset](https://www.kaggle.com/datasets/agungpambudi/trends-product-coffee-shop-sales-revenue-dataset). It contains transactional data for a fictional coffee shop chain, *Maven Roasters*, covering the period **January 2023 to June 2023**.  \
\
**Key Columns:**\
- `transaction_id` \'96 Unique identifier for each transaction  \
- `transaction_date` \'96 Date of the transaction  \
- `transaction_time` \'96 Time of the transaction  \
- `store_id` / `store_location` \'96 Location of the coffee shop  \
- `product_id` \'96 Unique product identifier  \
- `product_category` / `product_type` / `product_detail` \'96 Product information  \
- `transaction_qty` \'96 Quantity of product sold  \
- `unit_price` \'96 Price per unit  \
\
**Derived Features (from analysis):**\
- `revenue` = `transaction_qty * unit_price`  \
- `hour_of_day`, `day_of_week`, `month` \'96 derived from `transaction_date` and `transaction_time`  \
\
---\
\
## Objective\
\
The goal of this analysis is to:\
1. Understand the sales trends and revenue patterns of the coffee shop.  \
2. Identify high-performing products, locations, and time periods.  \
3. Provide actionable insights to optimize product mix, store performance, and potential promotions.  \
\
---\
\
## Observations\
\
- The dataset spans **Jan 2023 \'96 Jun 2023**, with no missing dates in the records.  \
- There is a **minor dip in revenue in February 2023**, which may require deeper investigation.  \
- **Barista Espresso** is consistently the top-selling product across all locations.  \
- **Total revenue by location** shows minimal variance, suggesting that the main drivers of revenue changes are likely at the **product level or external factors**.  \
\
---\
\
## Suggestions\
\
1. **Menu Optimization**  \
   - Focus on the top-selling products and consider reducing the number of low-selling items.  \
   - Redesign the menu to highlight high-revenue items.  \
\
2. **Inventory & Promotions**  \
   - To avoid inventory losses, offer targeted discounts on slower-moving products.  \
   - Track discounts and promotions in future datasets to better assess their impact on revenue.  \
\
3. **Data Enrichment**  \
   - Incorporate additional data such as **discounts, promotions, footfall, and holidays** to gain deeper insights.  \
   - Track revenue patterns by hour-of-day, day-of-week, and month to capture temporal trends.  \
\
---\
\
## Next Steps\
\
- Aggregate and analyze revenue at the **transaction level** or **per product**, rather than total daily revenue, to capture more variation.  \
- Apply **statistical modeling (linear regression)** and **machine learning models (Random Forest)** to understand the impact of different features on revenue.  \
- Explore **visualizations** like heatmaps, boxplots, and time series plots for better insight into product and store performance.\
}
