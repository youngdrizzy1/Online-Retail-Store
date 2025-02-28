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
- **Exploratory Data Analysis (EDA)**
- **Feature Engineering**
- **Customer Segmentation** (RFM Analysis & Clustering)
- **Predictive Classification Model**
- **Clustering Analysis (K-Means Clustering)**
- **Sales Forecasting (Time Series Analysis using Prophet)**
- **Marketing Strategy Recommendations**

## TOOLS AND TECHNOLOGIES
- **Python** (pandas, numpy, matplotlib, seaborn, scikit-learn, XGBoost, Prophet)
- **Jupyter Notebook** for data analysis and visualization
- **Machine Learning Models:** Decision Trees, Random Forest, XGBoost, Logistic Regression
- **Clustering Techniques:** K-Means Clustering
- **Time Series Analysis:** Facebook Prophet for sales forecasting

## EXPLORATORY DATA ANALYSIS (EDA)
### Summary Statistics and Data Insights
- Identified sales trends over time (yearly, quarterly, and monthly patterns).
- Examined customer purchase behavior based on days of the week and times of the day.
- Visualized top-selling products and purchase frequency.
- Analyzed customer retention based on Recency, Frequency, and Monetary (RFM) metrics.

## FEATURE ENGINEERING
- **Created new features:**
  - **Total Sales** = Quantity Sold × Unit Price
  - **Purchase Period:** Morning, Afternoon, Evening classification
  - **Days of the Week Analysis**
- **Outlier Detection and Handling:** Used IQR method to remove anomalies.
- **Feature Scaling & Encoding:** Standardization and categorical variable encoding.

## PREDICTIVE CLASSIFICATION MODEL
- **Machine Learning Models Used:**
  - Logistic Regression
  - Random Forest
  - XGBoost
- **Model Evaluation:**
  - Accuracy, Precision, Recall, F1-score
  - Feature importance analysis
  - Addressed class imbalance with resampling techniques

## CLUSTERING ANALYSIS
### Customer Segmentation (K-Means Clustering)
- **Performed RFM Analysis:**
  - **Recency:** How recently a customer purchased
  - **Frequency:** How often a customer buys
  - **Monetary Value:** How much a customer spends
- **Segmented Customers into Groups:**
  - High-Value Customers
  - Regular Buyers
  - One-Time Shoppers
- **Visualized Customer Clusters** to understand patterns and marketing opportunities.

## SALES FORECASTING
### Time Series Forecasting using Facebook Prophet
- **Trained model on historical sales data** to predict future revenue.
- **Created future time periods** and forecasted sales for the next months.
- **Visualized forecast trends** with confidence intervals.
- **Evaluated Model Accuracy** using RMSE and MAPE.

## CUSTOMER SEGMENTATION REPORT
- Identified key customer groups based on spending habits.
- Developed tailored marketing strategies for each segment.
- Recommended inventory adjustments to align with high-demand periods.

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

This structured report provides a comprehensive overview of the analysis conducted and the business implications derived from the data. The next step is preparing the presentation slides to summarize these findings effectively.
