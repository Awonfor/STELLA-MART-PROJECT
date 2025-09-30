# STELLA MART SALES COMPARISON KPI


## Background of Stellar Mart Corporation
- Founded in 2015, Stellar Mart is a rapidly growing mid-sized supermarket chain operating across three major cities in Myanmar (Yangon, Mandalay, and Naypyitaw). 
- The company has positioned itself as a customer-centric retailer offering a diverse range of products across six carefully curated product lines: Food and Beverages, Fashion Accessories, Electronic Accessories, Sports and Travel, Home and Lifestyle, and Health and Beauty.
- Stellar Mart distinguishes itself through its innovative dual-tier customer engagement strategy. 
- The company offers a membership program called "Stellar Rewards," which provides exclusive benefits to registered members while also maintaining a welcoming environment for normal customers with purchasing patterns varying notably between genders and membership status. 
- From an operational perspective, Stellar Mart carefully tracks its financial metrics, including Cost of Goods Sold (COGS), gross margin percentages, gross income across all product lines and branches, and accepts three payment methods: Cash, credit cards, and E-wallets. 
<img width="11059" height="183" alt="image" src="https://github.com/user-attachments/assets/1d589b7d-8516-44de-93f0-1e09e13429f4" />

## Problem Statement 
 In 2019, Stellar Mart faced increasing competition in Myanmar's retail sector while experiencing inconsistent performance across its three city locations. Despite implementing a membership program and diverse payment options, the company observed varying levels of customer engagement, fluctuating sales patterns, and differing profitability metrics across product line. Management needed to understand why certain branches outperform others and how customer preference influence revenue generation.
<img width="8782" height="183" alt="image" src="https://github.com/user-attachments/assets/33897035-93fa-426d-a71d-9e1f7ea04607" />

## DataSet Used
- <a href="https://github.com/Awonfor/STELLA-MART-PROJECT/blob/main/Stellar%20Mart%20Corporation.csv">Dataset</a>
### Data Souce 
- <a href="https://www.kaggle.com/datasets">Kaggle</a>

## Tools Used
- Excel    : Data Cleaning and Preprocessing
- SQL      : Data Validation and querying
- Power BI : Data Visualization and Dashboard Creation

  
## Dataset Insight
- The Stellar Mart Corporation dataset from 2019 captures detail retail transactions across three Myanmar cities (Yangon, Mandalay, and Naypyitaw). Providing comprehensive insights into the supermarket chain's operations, customer behavior, and business performance. comprising the following columns
-   Customer type (Member/Non-Member),
-   Gender demographics,
-   Product Line: (Food and Beverages, Fashion Accessories, Electronic Accessories, Sports and Travel, Home and Lifestyle, Health and Beauty),
-   Unit Price: Price per unit sold,
-   Quantity
-   5% Tax
-   Total
-   COGs
-   Gross Margins
-   payment methods (Cash, Credit card, E-wallet),
-   Customer satisfaction ratings (1-10 scale);
  

# Key Performance Indicators
  ## KPI & metrics

- Same-Store Sales Growth Rate (comparing each city’s month-over-month performance)
     - DAX: SSGR = DIVIDE( [Current Month Sales] - [Previous Month Sales], [Previous Month Sales],0)
-  Member Value Ratio (%) =
     - DAX: MVR = Member Value Ratio = ([Total Member Revenue]/[Total Revenue]) 
-  Product Line Contribution to Total Revenue (%) =
     - DAX: Product Contribution % = DIVIDE([Total Revenue],CALCULATE([Total Revenue],ALL('Main Tables'[Product_line])),0) 
-  Customer Satisfaction Index (CSI) =
     - DAX: CSI = DIVIDE([Total Ratings], [Total Responses]*[Max Rating])
-  Payment Method Efficiency Ratio =
     - DAX: Payment Method Efficiency Ratio = [Efficient Payment Transaction] / [Transaction Count]

## Workflow
- Management needed to understand why certain branches outperform others and how customer preference influence revenue generation
- Imported Raw Data from <a href="https://www.kaggle.com/datasets">Kaggle</a>
- Data Cleaning – Removed duplicate records, replaced inconsistent text values in some columns and handled missing values to ensure dataset completeness in Excel
- Data Validation – Imported the clean excel file in to SQL for data validation.
- Visualization – Built interactive dashboards in Power BI featuring drillthrough pages, Custom highly advanced interractive tooltips and hierarchical drill-down/up functionality to enable detailed data exploration and actionable insights.
### Project Model
<img width="501" height="379" alt="Stellar Mart Model" src="https://github.com/user-attachments/assets/d4351a7f-8cfe-4b7e-bdb8-87ff5328fbee" />


## VISUALIZATION 
Power BI is an industry-leading business intelligence platform by Microsoft that I use to design and deploy dynamic, data-driven dashboards and reports. With deep integration capabilities across diverse data sources, Power BI enables efficient data modeling, real-time analytics, and interactive visual storytelling. My projects leverage Power BI’s advanced features—such as DAX, Power Query, and custom visuals—to deliver actionable insights and support data-informed decision-making at scale.

### DASHBOARD (Group Level Performance) 

https://github.com/user-attachments/assets/f64594a0-a4c1-4c12-8c79-d877e717b3f7

 <img width="683" height="386" alt="Exec Dashboard Updated" src="https://github.com/user-attachments/assets/1906d2f3-403e-490f-81d8-7a0ca9b89d81" />


#### Key Insights
##### Positive Insights

 - Customer Satisfaction: The gauge visual indicates a customer satisfaction rate of 69.8%, reflecting a generally positive perception of service quality.
 - Membership Impact: Card visuals on the dashboard show that members contribute 103.5% of total revenue and account for 50.8% of transaction value, highlighting the strong impact of the membership program on sales performance.
 - Payment Efficiency: While cash remains the highest revenue generator, credit card transactions demonstrate greater operational efficiency and consistency.
 - Product Performance: Stacked column charts reveal that Food & Beverages lead revenue generation, followed by Sports, Electronics, Fashion, and Lifestyle indicating a strong product category hierarchy.
##### Negative Insights
 - Store-Level Volatility: Line chart analysis shows that all three stores experienced a significant dip in February 2019, with Store A most severely impacted. Although there was recovery in March, Store B's rebound was notably slower than the others.
 - Product Line Imbalance: Categories such as Health & Beauty and Lifestyle underperform relative to top contributors, suggesting untapped growth opportunities.

#### Recommendations
 - Store Performance Optimization: Conduct root cause analysis for Store A’s volatility and implement localized promotions or operational changes. For Store B, introduce targeted growth strategies to accelerate performance recovery.
 - Expand Membership Leverage: Strengthen the membership program by introducing tiered rewards, personalized offers, and retention initiatives to further enhance its already substantial revenue contribution.
 - Drive Efficient Payments: Promote credit card usage through incentives like discounts or cashback to align high revenue with greater operational efficiency.
 - Refocus Product Strategy: Increase marketing efforts in high-performing categories such as Food & Beverages, while implementing cross-sell and bundling strategies in underperforming lines like Health & Beauty.
 - Implement Proactive Monitoring: Establish monthly KPI tracking at the store level to quickly identify performance drops and deploy corrective actions in real time.

## Branch Level Performance 
  ### Store A (Yangon)
  
<img width="683" height="385" alt="Store A insight Updated" src="https://github.com/user-attachments/assets/0250f56d-c84a-459d-9da6-81587face1c6" />

        
#### Key Insights
##### Positive Insights
 - Customer Satisfaction (Gauge Visual): Satisfaction stands at 70.4%, indicating strong service perception and opportunity for deeper engagement.
 - Membership Performance (Card Visuals, Member Value Ratio & Member Revenue Ratio): Members contribute 102.04% of total revenue and represent 50.5% of value, demonstrating the effectiveness of the loyalty program in driving revenue.
 - Digital Payment Preference (Stacked Bar Chart – Payment Method Revenue):E-wallets lead in usage, showing strong customer adoption of digital payments.
##### Negative Insights
 - Sales Volatility (Line Chart – Monthly Same Store Growth Rate): A sharp dip in February 2019 followed by recovery in March signals inconsistent sales performance, potentially affecting forecasting and planning.
 - Category Concentration Risk (Stacked Column Chart – Product Line Revenue + Card Visual & Top Selling Product): Home & Lifestyle is the top-selling category at Store A but is underperforming at the group level, posing a risk due to over-reliance on a weaker segment.
 - Profitability Mismatch (Payment Method Revenue – Stacked Bar Chart): While E-wallets generate the most revenue, credit cards offer higher efficiency and profitability, highlighting a gap between customer preference and business optimization.
 - Retention Risk (Combination of Gauge + Line Chart): Although customer satisfaction is high, continued sales volatility may weaken loyalty if not proactively addressed.
##### Recommendations
 - Broaden Product Strategy (Based on Product Line Revenue): Reduce dependence on Home & Lifestyle by cross-selling high-performing categories like Food & Beverages.
 - Stabilize Sales Patterns (Informed by Monthly Growth Rate Chart): Introduce recurring monthly promotions to smooth out dips and maintain steady growth.
 - Optimize Payment Mix (Based on Payment Method Revenue Chart): Promote credit card usage through incentives (e.g., discounts, cashback, loyalty points) to improve profitability while maintaining user convenience.
 - Upsell Loyal Customers (Leveraging Membership & Satisfaction KPIs): Use strong satisfaction and loyalty data to upsell members into higher-margin categories, increasing customer lifetime value.

   
### Store B (Mandalay)
<img width="682" height="383" alt="Store B Insight updated" src="https://github.com/user-attachments/assets/b2d33c15-2a46-48b7-a8e0-1e5c40a7a24d" />

#### Key Insights 
##### Positive Insights
 - Balanced Payment Distribution (Stacked Bar Chart – Payment Method Revenue): Revenue is evenly split across credit card ($37K), cash ($35K), and e-wallet ($34K), reflecting strong availability of customer payment options and digital adoption.
 - Strong Membership Performance (Card Visuals – Member Value Ratio & Revenue Ratio): Members represent 50.6% of value and contribute 102.31% of revenue, reinforcing the ongoing strength of loyalty-driven sales.

 ##### Negative Insights
 - Minimal Growth (Card Visual – Growth Rate & Line Chart – Monthly Growth): Store B has the lowest growth rate at 0.5%, with only a slight rebound in March following February’s decline, suggesting persistently weak momentum.
 - Category Instability (Card Visual – Top Selling Product Line & Column Chart – Product Line Revenue): Sports & Travel is the top-selling product, but its seasonal nature contributes to revenue volatility, making it a less stable primary driver.
 - Low Customer Satisfaction (Gauge Visual – Customer Satisfaction): At 68.2%, Store B reports the lowest satisfaction rate among all branches, increasing the risk of customer churn.
 - Stagnant Revenue Despite Options (Payment Method Revenue + Overall Revenue KPI): Even with a diverse mix of payment options, total revenue remains flat, signaling low customer engagement or weak promotional traction.

 ##### Recommendations
 - Improve Customer Engagement (Based on Satisfaction Gauge & Growth Trend): Enhance service quality and deliver personalized offers or loyalty perks to boost satisfaction and repeat visits.
 - Category Rebalancing (Product Line Revenue Insight): Reduce over-dependence on seasonal categories like Sports & Travel by actively promoting stable, higher-margin lines such as Food & Beverages and Fashion Accessories.
 - Local Market Campaigns (Based on Branch/City Filters): Launch location-specific promotions for Mandalay, targeting regional preferences to drive membership engagement and conversion.
 - Accelerate Growth (Using Overall KPI and Trends): Deploy aggressive sales strategies or local partnerships to push revenue beyond the current stagnation and capture untapped market share.

 ### Store C (Naypyitaw)
<img width="683" height="385" alt="Store C Insight Updated" src="https://github.com/user-attachments/assets/c42011ca-71c4-460d-8de4-6bdf3d636b88" />


#### Key Insights
##### Positive Insights
 - Moderate Growth Momentum (Card Visual – Growth Rate & Line Chart – Monthly Same Store Growth Rate): Store C posted a 12.9% growth rate, outperforming Store B’s flat trend, with signs of recovery in March after February’s dip.
 - Category Leadership (Card Visual – Top Selling Product Line & Column Chart – Product Line Revenue): Food & Beverages is the top-selling product line ($24K), consistent with group-wide success and serving as a reliable revenue driver.
 - High Customer Satisfaction (Gauge Visual – Customer Satisfaction): At 70.6%, satisfaction is one of the strongest among branches, indicating a positive customer experience.
 - Robust Membership Contribution (Card Visuals – Member Value Ratio & Member Revenue Ratio): Members represent 51.4% of value and contribute 105.95% of revenue, showing loyalty programs are effectively driving sales.

##### Negative Insights
 - Growth Gap vs. Store A (Card Visual – Growth Rate & Line Chart – Monthly Same Store Growth Rate): While growth is positive, Store C underperforms compared to Store A’s 26.1%, highlighting missed scaling opportunities.
 - Revenue Scale Lag (Column Chart – Product Line Revenue): Despite Food & Beverages leading, total revenue lags behind Store A, signaling slower market capture.
 - Over-Reliance on Cash (Stacked Bar Chart – Payment Method Revenue): Cash dominates transactions ($43K), reducing Efficiency compared to credit card usage.
 - Underperformance in Other Categories (Column Chart – Product Line Revenue): Electronics ($19K), fashion accessories ($22K), and lifestyle ($14K) trail far behind F&B, revealing weak diversification.

##### Recommendations
 - Scale Core Category Strength (Product Line Revenue Insight): Intensify Food & Beverage promotions through bundles, seasonal deals, and loyalty-based incentives to cement leadership and boost revenue.
 - Optimize Payment Mix (Payment Method Revenue Insight): Introduce credit card incentives such as cashback or member-only discounts to reduce cash dependence and improve margins.
 - Broaden Product Portfolio (Product Line Revenue Insight): Actively promote electronics and fashion accessories with cross-selling strategies and targeted campaigns to reduce over reliance on Food & Beverages.
 - Maximize Membership Impact (Customer Satisfaction & Membership Ratio Cards): Launch exclusive member-only campaigns, referral bonuses, and early-access offers to deepen loyalty and increase transaction sizes.
## BUSINESS SOLUTION (Group + Branch)
-  Stabilize Growth: Smooth sales volatility with consistent campaigns and seasonal product balancing.
-  Boost Store B: Urgent focus on service quality, customer engagement, and category rebalancing.
-  Optimize Payments: Shift customers from cash/e-wallet toward credit cards with targeted incentives.
-  Leverage Memberships: Expand loyalty-driven offers to sustain the revenue edge across all stores.
-  Product Strategy: Double down on Food & Beverages while cross-selling underperforming categories.



















