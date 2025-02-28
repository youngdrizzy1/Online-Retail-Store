# ONLINE RETAIL STORE ANALYSIS

## Table of Contents
- [Introduction](#INTRODUCTION)
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

### 2. Business Problem
Understanding customer buying behavior enables businesses to make data-driven decisions. The key objectives are:
- **Customer Segmentation:** Grouping customers for targeted marketing strategies.
- **Inventory Optimization:** Stocking high-demand products efficiently while avoiding overstocking of low-demand products.
- **Revenue Growth:** Forecasting future sales trends to improve decision-making.
- **Marketing Strategies:** Personalized recommendations and promotional campaigns based on purchasing behavior.

### 3. Methodology
A structured data science approach was followed, including:
1. **Data Collection & Preprocessing**
   - Used **Excel** for initial data exploration to detect abnormalities.
   - **Dataset was downloaded as part of the task, not gathered manually.**
   - Used **Python** to clean missing values, handle duplicates, and divide the data into three parts:
     - **Successful Products Sold**
     - **Product Returns**
     - **Logistics**
   - **Outliers were handled during the clustering analysis, not initial preprocessing.**

2. **Exploratory Data Analysis (EDA)**
   - Analyzed purchase trends over time (yearly, quarterly, monthly).
   - Identified top-selling products and customer purchase behavior.
   - Used visualizations to uncover sales patterns.

3. **Feature Engineering**
   - Created new features (e.g., Total Sales, Purchase Period, Days of the Week).
   - Applied encoding techniques for categorical variables.
   - Normalized and standardized numerical data for better model performance.

4. **Customer & Product Segmentation (Using RFM & Clustering)**
   - Performed Recency, Frequency, and Monetary (RFM) analysis.
   - Applied **K-Means clustering** to group customers into meaningful segments (**classified as 0, 1, 2**).
   - Identified high-value customers, regular buyers, and one-time shoppers.
   - Conducted **product segmentation** to categorize items based on sales trends and demand patterns.

5. **Predictive Classification Model**
   - Implemented machine learning models (Logistic Regression, Random Forest, XGBoost).
   - Trained models to classify transactions based on customer purchasing behavior.
   - Evaluated performance using accuracy, precision, recall, and F1-score.

6. **Clustering Analysis**
   - Used unsupervised learning (**K-Means**) for **customer segmentation and product segmentation.**
   - Determined optimal clusters using the Elbow method and silhouette score.
   - **Outliers were handled at this stage, not earlier.**

7. **Sales Forecasting (Time Series Analysis)**
   - Applied **Facebook Prophet** to predict future sales trends.
   - Evaluated forecast accuracy using RMSE and MAPE.
   - Provided insights into expected revenue trends for strategic decision-making.

8. **Business Insights & Marketing Strategy Recommendations**
   - Suggested personalized marketing campaigns for different customer segments.
   - Recommended stock optimization strategies based on demand forecasting.
   - Proposed targeted promotions to boost sales for specific product categories.
   - Suggested engagement strategies for one-time buyers to improve retention.

## TOOLS AND TECHNOLOGIES
- **Excel** for initial data exploration and anomaly detection.
- **Python** (pandas, numpy, matplotlib, seaborn, scikit-learn, XGBoost, Prophet).
- **Jupyter Notebook** for data analysis and visualization.
- **Machine Learning Models:** Decision Trees, Random Forest, XGBoost, Logistic Regression.
- **Clustering Techniques:** K-Means Clustering.
- **Time Series Analysis:** Facebook Prophet for sales forecasting.

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
