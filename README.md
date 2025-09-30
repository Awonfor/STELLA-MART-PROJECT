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
-  Product Line Contribution To Total Revenue (%) =
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

<img width="501" height="379" alt="Stellar Mart Model" src="https://github.com/user-attachments/assets/d4351a7f-8cfe-4b7e-bdb8-87ff5328fbee" />


## VISUALIZATION 
Power BI is an industry-leading business intelligence platform by Microsoft that I use to design and deploy dynamic, data-driven dashboards and reports. With deep integration capabilities across diverse data sources, Power BI enables efficient data modeling, real-time analytics, and interactive visual storytelling. My projects leverage Power BI’s advanced features—such as DAX, Power Query, and custom visuals—to deliver actionable insights and support data-informed decision-making at scale.

### DASHBOARD (Group Level Performance) 


 <img width="683" height="386" alt="Exec Dashboard Updated" src="https://github.com/user-attachments/assets/1906d2f3-403e-490f-81d8-7a0ca9b89d81" />


#### Key Insights
#####Positive Insights

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

        
#### Key Insights (Concerns)
-  Growth rate dropped sharply in February, though March showed recovery. This signals volatility in sales performance.
-  Top product line = Home & Lifestyle, but this category is lower-performing at the group level. This is a  risk of over-dependence on a weaker product line.
-  Payment preference is E-wallet, yet efficiency analysis shows credit cards are more profitable. Mismatch between customer preference and profitability.
-  Customer satisfaction is relatively high (70.4%), but sales volatility may eventually erode loyalty.
  
#### Recommendations
 -  Diversify product focus: Cross-sell food & beverages (the group’s strongest product line) to reduce over-reliance on home & lifestyle.
 -  Stabilize sales cycles: Introduce consistent monthly promotions to smooth out dips like February.
 -  Payment optimization: Offer targeted incentives (e.g., discounts, loyalty points) to encourage credit card adoption.
 -  Retention focus: Leverage high customer satisfaction by upselling members into higher-value categories.

### Store B (Mandalay)
<img width="682" height="383" alt="Store B Insight updated" src="https://github.com/user-attachments/assets/b2d33c15-2a46-48b7-a8e0-1e5c40a7a24d" />

#### Key Insights (Concerns)
-  Weakest performer → only 0.5% growth rate, barely recovering after February.
-  Top product line = Sports & Travel, but this is a seasonal/volatile category → explains unstable revenue growth.
-  Customer satisfaction is lowest (68.2%) among branches → risk of churn.
-  Payment split is more balanced (credit card $37K, cash $35K, e-wallet $34K), but revenue remains stagnant → customer engagement is low despite available options.

#### Recommendations
-  Customer engagement: Improve satisfaction through service quality and personalized offers.
-  Category rebalancing: Promote higher-margin, stable product lines (e.g., food & beverages, fashion accessories) alongside sports & travel.
-  Local campaigns: Tailor promotions to Mandalay’s customer base to boost participation and membership engagement.
-  Growth push: Aggressive sales campaigns or partnerships are needed to lift growth beyond stagnation.

 ### Store C (Naypyitaw)
<img width="683" height="385" alt="Store C Insight Updated" src="https://github.com/user-attachments/assets/c42011ca-71c4-460d-8de4-6bdf3d636b88" />


#### Key Insights 
-  Moderate performance with 12.9% growth rate (better than Store B but weaker than Store A’s 26.1%).
-  Top product line = Food & Beverages, aligning with group-wide success, but still underperforming compared to Store A’s revenue scale.
-  Cash dominates payments ($43K), which is less efficient than credit cards, showing reliance on low-margin payment methods.
-  Customer satisfaction is high (70.6%), and membership contribution is strong (105.9%) → growth potential exists, but product mix is not fully optimized.
  
  #### Recommendations
-  Capitalize on strong category: Expand Food & Beverage promotions to further scale revenue in Naypyitaw.
-  Shift payment behavior: Encourage credit card/e-wallet use to improve efficiency and profitability.
-  Revenue diversification: Push growth in electronics and fashion accessories to balance product portfolio.
-  Scale loyalty impact: Leverage strong membership performance by rolling out exclusive member-only campaigns.

## Management Priorities (Group + Branch)
-  Stabilize Growth: Smooth sales volatility with consistent campaigns and seasonal product balancing.
-  Boost Store B: Urgent focus on service quality, customer engagement, and category rebalancing.
-  Optimize Payments: Shift customers from cash/e-wallet toward credit cards with targeted incentives.
-  Leverage Memberships: Expand loyalty-driven offers to sustain the revenue edge across all stores.
-  Product Strategy: Double down on Food & Beverages while cross-selling underperforming categories.



















