# ONLINE RETAIL STORE ANALYSIS

## Table of Contents
- [Introduction](#INTRODUCTION)
- [Dataset Overview](#DATASET-OVERVIEW)
- [Data Quality Assessment](#DATA-QUALITY-ASSESSMENT)
- [Tools & Technologies Used](#TOOLS-AND-TECHNOLOGIES)
- [Exploratory Data Analysis (EDA)](#EDA)
- [Feature Engineering](#FEATURE-ENGINEERING)
- [Visualization](#VISUALIZATION)
- [Predictive Classification Model](#PREDICTIVE-CLASSIFICATION-MODEL)
- [Clustering Analysis](#CLUSTERING-ANALYSIS)
- [Sales Forecasting](#SALES-FORECASTING)
- [Customer and Product Segmentation](#CUSTOMER-SEGMENTATION-REPORT)
- [Business Insights & Marketing Strategy Recommendations](#BUSINESS-INSIGHTS-AND-MARKETING-STRATEGY-RECOMMENDATIONS)
- [Conclusion](#CONCLUSION)
- [Recommendations](#RECOMMENDATIONS)

## INTRODUCTION
### Objective
The objective of this project is to develop a predictive model that categorizes online shopping transactions into certain categories and clusters. Based on machine learning and clustering techniques, the model will allow companies to uncover hidden patterns, make inventory management problems easier, improve customer segmentation, and improve sales forecasts.

## DATASET OVERVIEW
The dataset used in this project is online retail transactions and contains the following primary columns:

- **InvoiceNo:** Unique transaction code.
- **StockCode:** Unique product code.
- **Description:** Name of product.
- **Quantity:** Units purchased.
- **InvoiceDate:** Date and time of transaction.
- **UnitPrice:** Cost per unit of product.
- **CustomerID:** Unique customer code (few missing values).
- **Country:** Country in which transaction was made.

## DATA QUALITY ASSESSMENT
### Identified Issues

**Missing Values:**
- 1,454 missing values in the Description column.
- 135,080 missing values in the CustomerID column.

**Negative Values:**
- 10,624 negative values in the Quantity column (indicating product returns).
- 2 negative values in the UnitPrice column.
  
**Zero Values:**
- 2,515 zero values in the UnitPrice column.
- Special Characters and Blanks:
- Special characters and blank values in the Description column.
  
**Duplicate Rows:**
- 5,268 duplicate rows.
  
**Unspecified Entries:**
- Some rows in the Country column had "unspecified" entries.
  
## Rectifying Issues
**Handling Missing Values:**
- CustomerID: Missing values were handled using forward fill.
- Description: Missing values were identified and handled.
  
**Removing Negative and Zero Values:**
- Removed negative Quantity values (product returns).
- Removed negative UnitPrice values and invalid entries.
- Filtered out zero UnitPrice values.
  
**Renaming "Unspecified" Country:**
- "Unspecified" country entries were renamed to "Unknown" for clarity.
  
**Removing Duplicates:**
- Dropped 5,268 duplicate rows to ensure data accuracy.
  
**Standardizing Product Descriptions:**
- Renamed the Description column to Product for consistency.

## TOOLS AND TECHNOLOGIES
- **Excel** for initial data exploration and anomaly detection.
- **Python** (pandas, numpy, matplotlib, seaborn, scikit-learn, XGBoost, Prophet).
- **Jupyter Notebook** for visualization and analysis.
- **Machine Learning Models:** Decision Trees, Random Forest, XGBoost, Logistic Regression.
- **Clustering Techniques:** K-Means Clustering.
- **Time Series Analysis:** Facebook Prophet to predict sales. 

## EXPLORATORY DATA ANALYSIS (EDA)


## FEATURE ENGINEERING
**Created new features:**
- Total Sales, Year
- Quarter
- Month
- Hour of the Day
- Period of the Day
- Days of the Week

## VISUALIZATION AND ISIGHTS
**Top Selling Products**
- Top-selling product: REGENCY CAKESTAND 3 TIER
- High demand for: Paper craft, home decor, and festive items
- Popular categories: T-light holders, bunting, lights, storage items
- Stocking strategy: Prioritize best-sellers, bundle related products
  
  ![1](https://github.com/user-attachments/assets/db66489b-641d-4ceb-a1d8-98dc48de95f2)

**Top 10 Countries by Sales**
- Dominant Market: United Kingdom has overwhelmingly the highest sales, far exceeding all other countries.
- Other Key Markets: Netherlands, EIRE (Ireland), Germany, and France follow, but with significantly lower sales.
- Global Reach: Sales extend beyond Europe to countries like Australia, Japan, and Switzerland.
- Potential Focus Areas: Expanding marketing efforts in top-performing international markets could drive more growth.

  ![2](https://github.com/user-attachments/assets/9c7e1a32-9bfa-448d-9e95-a9788871d415)

**Daily Purchase Trend**
- Highest sales occur on Tuesday and Thursday, with peaks above 2 million.
- Sales drop significantly on Saturday, reaching near zero, which suggests minimal or no transactions on this day.
- Sales slightly recover on Sunday but remain lower compared to weekdays.
- Overall, weekdays have higher sales than weekends, indicating that most transactions happen during the workweek.

  ![5](https://github.com/user-attachments/assets/c8bbb3f7-02b2-413a-b83a-ed0d5633e580)

**Period Of The Day Purchase Trends**
- Afternoon has the highest sales, peaking around 6 million.
- Morning follows closely, with sales above 4 million.
- Sales drop significantly in the evening, suggesting fewer transactions.
- Night has the lowest sales, almost negligible, indicating little to no business activity.

  ![6](https://github.com/user-attachments/assets/5b92f5ce-8291-47e2-9a98-0a1d344e3165)

**Monthly Purchase Trend**
- Slow Start: Sales are relatively low in January and February, with fluctuations in the first half of the year.
- Steady Growth: Sales pick up from May to August, though with slight variations.
- Peak Season: Significant sales increase from September onward, peaking in November and December—likely due to holiday shopping.
- Possible Strategy: Capitalizing on peak months (November-December) with promotions and stock optimization could maximize revenue.

  ![3](https://github.com/user-attachments/assets/3c0b44c6-ee95-4e31-8844-15a18987e7e6)

**Quarter of the year trend**
- Gradual Growth: Sales increase steadily from Q1 to Q3, indicating a consistent upward trend.
- Major Surge in Q4: A sharp rise in Q4 sales, likely due to holiday shopping (Black Friday, Christmas).
- Strategic Focus:
  - Boost marketing and inventory for Q4 to maximize sales.
  - Identify ways to improve performance in Q1 and Q2 (e.g., seasonal promotions).
 
  ![4](https://github.com/user-attachments/assets/6ff1d401-94d3-4121-a202-06dd05bb5649)

## PREDICTIVE CLASSIFICATION MODEL
- Applied machine learning algorithms (Logistic Regression, Random Forest, XGBoost).
- Trained models to forecast customer buying behavior for transaction classification.
- Compared the performance with accuracy, precision, recall, and F1-score.

## CLUSTERING ANALYSIS
- Used unsupervised learning (**K-Means**) for **product segmentation and customer segmentation.**
- Determined best clusters with the help of the Elbow method and silhouette score.
- **Outliers were handled here, not earlier.**

## SALES FORECASTING (TIME SERIES ANALYSIS)
- Used **Facebook Prophet** to predict future sales trends.
- Compared the accuracy of the forecasts with RMSE and MAPE.
- Provided insights into expected revenue trends for strategic decision-making.

## BUSINESS INSIGHTS & MARKETING STRATEGY RECOMMENDATIONS
- Personalized marketing strategies based on customer segments.
- Dynamic pricing and discounting strategies to maximize revenue.
- Inventory restocking recommendations based on predictive insights.
- Customer loyalty programs to retain high-value customers.
- Targeted engagement strategies to convert one-time buyers into repeat customers.

## CONCLUSION
- Data-driven insights enable businesses to optimize their sales strategies.
- Predictive modeling improves transaction classification and inventory management.
- Clustering analysis helps in precise customer targeting for marketing efforts.
- Sales forecasting provides future revenue estimates for better planning.

## RECOMMENDATIONS
1. **Target High-Value Customers:** Offer loyalty rewards and exclusive promotions.
2. **Stock Management Optimization:** Reduce overstocking and maintain high-demand product availability.
3. **Improve Marketing Campaigns:** Personalize recommendations based on customer clusters.
4. **Monitor Sales Trends:** Use sales forecasting insights for proactive decision-making.
5. **Enhance Customer Retention:** Identify customers at risk and implement engagement activities.
6. **Convert One-Time Buyers into Repeat Buyers:** Develop engagement strategies such as email reminders and special discounts.
