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
### 1. Objective
The purpose of this project is to design a predictive model that categorizes online shopping transactions into certain categories and clusters. Utilizing machine learning and clustering techniques, the model will help businesses identify hidden patterns, reduce inventory management complexities, improve customer segmentation, and enhance sales forecasting.

## DATASET OVERVIEW
The dataset used in this project consists of online retail transactions and contains the following key columns:

- **InvoiceNo:** Unique identifier for each transaction.
- **StockCode:** Unique product identifier.
- **Description:** Product name.
- **Quantity:** Number of products purchased.
- **InvoiceDate:** Date and time of the transaction.
- **UnitPrice:** Price per product unit.
- **CustomerID:** Unique identifier for each customer (some missing values).
- **Country:** Country where the transaction occurred.

## DATA QUALITY ASSESSMENT
Before performing any analysis, a data quality check was conducted to identify key issues:

1. **Missing Values:**
   - CustomerID was missing for several transactions.
   - Some product descriptions were missing.

2. **Duplicate Entries:**
   - Identified and removed duplicated rows to ensure data accuracy.

3. **Negative & Zero Values:**
   - Some transactions had negative quantities, indicating **product returns**.
   - Zero and negative prices were identified and handled accordingly.

4. **Special Characters & Formatting Issues:**
   - Some product descriptions contained special characters, which were cleaned.

5. **Unspecified Countries:**
   - Some transactions lacked country information, requiring further review.

## TOOLS AND TECHNOLOGIES
- **Excel** for initial data exploration and anomaly detection.
- **Python** (pandas, numpy, matplotlib, seaborn, scikit-learn, XGBoost, Prophet).
- **Jupyter Notebook** for data analysis and visualization.
- **Machine Learning Models:** Decision Trees, Random Forest, XGBoost, Logistic Regression.
- **Clustering Techniques:** K-Means Clustering.
- **Time Series Analysis:** Facebook Prophet for sales forecasting.

## DATA COLLECTION & PREPROCESSING
A structured data preprocessing approach was followed to clean and prepare the dataset:

1. **Handling Missing Values:**
   - Transactions with missing **CustomerID** were either imputed or excluded based on their relevance.
   - Missing product descriptions were replaced using **StockCode mappings**.

2. **Removing Duplicates:**
   - Identified duplicate transactions and removed them to prevent redundancy.

3. **Dealing with Negative & Zero Values:**
   - Negative values in the **Quantity** column were treated as product returns.
   - Transactions with zero or negative **UnitPrice** were reviewed and handled.

4. **Standardizing Text Data:**
   - Removed special characters from product descriptions.
   - Converted text data to lowercase for consistency.

5. **Date Formatting & Extraction:**
   - Converted **InvoiceDate** to proper datetime format.
   - Extracted features like **Year, Month, Day, and Hour of Purchase**.

## EXPLORATORY DATA ANALYSIS (EDA)
- Analyzed purchase trends over time (yearly, quarterly, monthly).
- Identified top-selling products and customer purchase behavior.
- Used visualizations to uncover sales patterns.

## FEATURE ENGINEERING
- Created new features (e.g., Total Sales, Purchase Period, Days of the Week).
- Applied encoding techniques for categorical variables.
- Normalized and standardized numerical data for better model performance.

## CUSTOMER & PRODUCT SEGMENTATION (USING RFM & CLUSTERING)
- Performed Recency, Frequency, and Monetary (RFM) analysis.
- Applied **K-Means clustering** to group customers into meaningful segments (**classified as 0, 1, 2**).
- Identified high-value customers, regular buyers, and one-time shoppers.
- Conducted **product segmentation** to categorize items based on sales trends and demand patterns.

## PREDICTIVE CLASSIFICATION MODEL
- Implemented machine learning models (Logistic Regression, Random Forest, XGBoost).
- Trained models to classify transactions based on customer purchasing behavior.
- Evaluated performance using accuracy, precision, recall, and F1-score.

## CLUSTERING ANALYSIS
- Used unsupervised learning (**K-Means**) for **customer segmentation and product segmentation.**
- Determined optimal clusters using the Elbow method and silhouette score.
- **Outliers were handled at this stage, not earlier.**

## SALES FORECASTING (TIME SERIES ANALYSIS)
- Applied **Facebook Prophet** to predict future sales trends.
- Evaluated forecast accuracy using RMSE and MAPE.
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
5. **Enhance Customer Retention:** Identify at-risk customers and implement engagement strategies.
6. **Convert One-Time Buyers:** Develop engagement tactics such as email follow-ups and special discounts.
