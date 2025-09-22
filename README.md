# STELLA MART SALES PERFORMANCE COMPARISON PROJECT

## Background of Stellar Mart Corporation
- Founded in 2015, Stellar Mart is a rapidly growing mid-sized supermarket chain operating across three major cities in Myanmar (Yangon, Mandalay, and Naypyitaw). 
- The company has positioned itself as a customer-centric retailer offering a diverse range of products across six carefully curated product lines: Food and Beverages, Fashion Accessories, Electronic Accessories, Sports and Travel, Home and Lifestyle, and Health and Beauty.
- Stellar Mart distinguishes itself through its innovative dual-tier customer engagement strategy. 
- The company offers a membership program called "Stellar Rewards," which provides exclusive benefits to registered members while also maintaining a welcoming environment for normal customers with purchasing patterns varying notably between genders and membership status. 
- From an operational perspective, Stellar Mart carefully tracks its financial metrics, including Cost of Goods Sold (COGS), gross margin percentages, gross income across all product lines and branches, and accepts three payment methods: Cash, credit cards, and E-wallets. 
<img width="11059" height="183" alt="image" src="https://github.com/user-attachments/assets/1d589b7d-8516-44de-93f0-1e09e13429f4" />

## Problem Statement 
- In 2019, Stellar Mart faces increasing competition in Myanmar's retail sector while experiencing inconsistent performance across its three city locations.
- Despite implementing a membership program and diverse payment options, the company observes varying levels of customer engagement, fluctuating sales patterns, and differing profitability metrics across product lines.
- Management needs to understand why certain branches outperform others and how customer preferences influence revenue generation.
<img width="8782" height="183" alt="image" src="https://github.com/user-attachments/assets/33897035-93fa-426d-a71d-9e1f7ea04607" />

## DataSet Used
- <a href="https://github.com/Awonfor/STELLA-MART-PROJECT/blob/main/Stellar%20Mart%20Corporation.csv">Dataset</a>
### Data Souce 
- <a href="https://www.kaggle.com/datasets">Kaggle</a>

## Dataset Insight
- The Stellar Mart Corporation dataset from 2019 captures detailed retail transactions across three Myanmar cities (Yangon, Mandalay, and Naypyitaw). comprising the following columns
-   Customer types (Member/Non-Member),
-   Gender demographics,
-   Six product lines (Food and Beverages, Fashion Accessories, Electronic Accessories, Sports and Travel, Home and Lifestyle, Health and Beauty),
-   Financial metrics (unit price, quantity, 5% tax, total amount, COGS, gross margins),
-   Three payment methods (Cash, Credit card, E-wallet),
-   Customer satisfaction ratings (1-10 scale);
- Providing comprehensive insights into the supermarket chain's operations, customer behavior, and business performance.

# Key Performance Indicators
  ## KPI & metrics

- Same-store sales growth rate (comparing each city’s month-over-month performance) =
      ((Current month sales – previous month sales) / Previous month Sales) * 100
-  Member Value Ratio (%) =
      (Total member revenue / Total revenue) * 100
-  Product Line Contribution To Total Revenue (%) =
      (Total Revenue / Revenue from product line) * 100
-  Customer Satisfaction Index (CSI) =
      Total ratings / (Response Count * Maximum Rating)
-  Payment Method Efficiency Ratio =
      Efficient Payment Transaction / Transaction Count

## Tools Used
- Excel; Data Cleaning and Preprocessing
- SQL; Data Validation and querying
- Power BI; Data Visualization and Dashboard Creation

## Workflow
- Import Raw Data from <a href="https://www.kaggle.com/datasets">Kaggle</a>
- Data Cleaning – removed duplicate records, replaced inconsistent text values in some columns and handled missing values to ensure dataset completeness in Excel
- Data Validation – validated dataset integrity using SQL queries
- Visualization – Built interactive dashboards in Power BI featuring drillthrough pages and hierarchical drill-down/up functionality to enable detailed data exploration and actionable insights.

## DASHBOARD (Group Level Performance) 


 <img width="683" height="386" alt="Exec Dashboard Updated" src="https://github.com/user-attachments/assets/1906d2f3-403e-490f-81d8-7a0ca9b89d81" />


  #### Key Insights 
-  Growth Trends: All three stores dipped in February 2019, with Store A hit hardest. Recovery occurred in March, but Store B’s rebound lagged behind others.
-  Customer Engagement: Customer satisfaction is above average (69.8%), showing healthy service perception.
-  Membership Program: Strong impact – members account for 50.8% of value and contribute 103.5% of revenue, driving more sales than non-members.
-  Payment Methods: While cash generates the highest revenue, efficiency analysis shows credit cards deliver better performance.
-  Product Performance: Food & beverages dominate revenue, followed by sports, electronics, fashion, and lifestyle categories.

#### Recommendations
-  Branch-Level Strategy: Investigate Store A’s volatility and Store B’s slower growth; tailor localized promotions to stabilize performance.
-  Leverage Memberships: Expand loyalty benefits and targeted campaigns to further capitalize on the revenue-driving member base.
-  Optimize Payments: Encourage credit card adoption through incentives (e.g., discounts, cashback) to balance efficiency with customer preferences.
-  Category Focus: Double down on food & beverages promotions, while improving cross-selling in underperforming product lines (e.g., health & beauty).
-  Continuous Monitoring: Track branch-level KPIs monthly to identify sales dips early and adjust strategies proactively.

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



















