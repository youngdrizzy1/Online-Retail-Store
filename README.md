# ONLINE RETAIL STORE ANALYSIS

## Table of Contents
- [Introduction](#INTRODUCTION)
- [Dataset Overview](#DATASET-OVERVIEW)
- [Data Quality Assessment](#DATA-QUALITY-ASSESSMENT)
- [Tools & Technologies Used](#TOOLS-AND-TECHNOLOGIES)
- [Exploratory Data Analysis (EDA)](#EDA)
- [Feature Engineering](#FEATURE-ENGINEERING)
- [Predictive Classification Model](#PREDICTIVE-CLASSIFICATION-MODEL)
- [Clustering Analysis](#CLUSTERING-ANALYSIS)
- [Sales Forecasting](#SALES-FORECASTING)
- [Customer Segmentation Report](#CUSTOMER-SEGMENTATION-REPORT)
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

## DATA COLLECTION & PREPROCESSING
A formal data preprocessing technique was followed to sanitize and normalize the data:

1. **Handling Missing Values:**
   - Transactions with absent **CustomerID** were replaced or removed based on their impact.
   - Missing product details were replaced by **StockCode mappings**.

2. **Removing Duplicates:**
   - Duplicate transactions were recognized and removed to exclude redundancy.

3. **Processing Negative & Zero Values:**
   - Negative quantities in the **Quantity** field were processed as product returns.
   - Transactions with zero or negative **UnitPrice** were checked and resolved.

4. **Text Data Normalization:**
   - Product description special characters were trimmed.
   - Text data were converted to lower case for standardization.

5. **Formatting & Extraction Dates:**
   - **InvoiceDate** was formatted into standardized datetime format.
- Extracted features like **Year, Month, Day, and Hour of Purchase**.

## EXPLORATORY DATA ANALYSIS (EDA)
- Compared purchase behaviors across time (yearly, quarterly, month by month).
- Established top-selling products and customer buying behavior.
- Used visualizations to expose sales patterns.

## FEATURE ENGINEERING
- Created new features (e.g., Total Sales, Purchase Period, Days of the Week).
- Used encoding techniques for categorical variables.
- Normalized and standardized numeric values for better model performance.

## CUSTOMER & PRODUCT SEGMENTATION (RFM & CLUSTERING)
- Performed Recency, Frequency, and Monetary (RFM) analysis.
- Applied **K-Means clustering** to segment customers into meaningful groups (**marked as 0, 1, 2**).
- Segmented high-value customers, frequent buyers, and occasional shoppers.
- Performed **product segmentation** to segment products based on sales patterns and demand trends.

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
