
Retail Sales & Profit Analysis
 Project Overview

An end-to-end Retail Sales & Profit Analysis project using Python to explore sales performance, profitability, product categories, customer segments, discounts, and transaction-level patterns.

The project demonstrates a practical Data Analyst workflow, starting with data loading and quality checks, followed by exploratory data analysis, business performance analysis, data visualisation, and a simple predictive analysis.

The main focus of the project is turning retail data into meaningful business insights and supporting data-driven decision-making.

 Business Objective

The objective of this project is to understand the key factors affecting retail sales and profitability and identify areas of strong and weak business performance.

The analysis focuses on:

Overall sales and profit performance
Product category and sub-category performance
Customer segment performance
Sales and profit distributions
Discount and profit relationships
Loss-making transactions and product areas
Relationships between key numerical variables
A simple introduction to Sales prediction
 Key Business Questions

The project investigates:

What are the overall Sales and Profit levels?
How are Sales and Profit distributed?
Which product categories generate the highest Sales?
Which categories generate the highest Profit?
Which sub-categories perform best?
Which customer segment generates the most Sales?
What is the relationship between Discount and Profit?
What is the relationship between Sales and Profit?
Which sub-categories have the lowest profitability?
How many transactions are loss-making?
Can basic transaction-level variables be used to estimate Sales?
 Project Workflow
Raw Retail Data
      ↓
Data Loading
      ↓
Data Understanding
      ↓
Data Quality Checks
      ↓
Exploratory Data Analysis
      ↓
Business Performance Analysis
      ↓
Data Visualisation
      ↓
Correlation Analysis
      ↓
Business Insights
      ↓
Simple Predictive Analysis
      ↓
Conclusion & Recommendations
 Technologies & Tools
Technology	Purpose
Python	Data analysis
Pandas	Data manipulation and analysis
NumPy	Numerical operations
Matplotlib	Data visualisation
Seaborn	Statistical visualisation
Scikit-learn	Simple predictive modelling
Google Colab	Development environment
GitHub	Portfolio and version control
1. Data Loading

The superstore.csv dataset is uploaded into Google Colab and loaded using Pandas.

uploaded = files.upload()


df = pd.read_csv("superstore.csv")

The first five records are displayed to confirm that the data has loaded correctly.

2. Data Understanding

The dataset is examined using:

Number of rows and columns
Column names
Data types
Dataset information
Initial observations

This provides an understanding of the structure of the data before analysis.

3. Data Quality Assessment

The project checks for:

Missing Values
df.isnull().sum()
Duplicate Records
df.duplicated().sum()

These checks help determine whether the dataset contains common data-quality issues.

 Exploratory Data Analysis
4. Business KPIs

Key performance indicators are calculated, including:

Total Sales
Total Profit
Total Transactions
Average Sales per Transaction
Average Profit per Transaction

These KPIs provide a high-level overview of business performance.

5. Descriptive Statistics

Descriptive statistics are calculated for:

Sales
Quantity
Discount
Profit

The analysis examines measures such as mean, standard deviation, minimum, maximum, and quartiles.

6. Sales & Profit Distribution

Histograms are used to examine the distribution of:

Sales
Profit

These visualisations help identify the concentration and spread of transaction values.

 Product Performance Analysis
7. Sales & Profit by Category

Sales, Profit, and transaction counts are aggregated by product category.

This helps identify which major product categories contribute most to overall business performance.

Visualisations are created for:

Total Sales by Category
Total Profit by Category
8. Sales & Profit by Sub-Category

The analysis goes into greater detail by examining individual product sub-categories.

The project identifies:

Top 10 sub-categories by Sales
Top 10 sub-categories by Profit
Lower-performing sub-categories

This provides more detailed information for product performance analysis.

 Cstomer Segment Analysis

Sales, Profit, and transaction counts are calculated for each customer segment.

The analysis identifies which customer segment contributes the greatest amount of Sales.

This can support decisions around customer targeting and commercial strategy.

Discount & Profit Analysis

A scatter plot examines the relationship between Discount and Profit.

This is an important business question because excessive discounting may affect profitability.

The analysis helps identify whether higher discounts are associated with lower or higher profit levels.

Sales & Profit Relationship

A scatter plot is used to investigate the relationship between Sales and Profit.

This helps determine whether higher sales values generally correspond to higher profitability.

 Correlation Analysis

A correlation matrix is created for:

Sales
Quantity
Discount
Profit

A heatmap provides a visual overview of the relationships between these variables.

Correlation is used as an exploratory tool and does not by itself establish causation.

 Loss-Making Transactions

Transactions with negative Profit are identified.

The project calculates:

Number of loss-making transactions
Total loss
Sub-categories with the lowest total Profit

This is particularly useful from a business perspective because high Sales do not necessarily mean high profitability.

Business Performance Summary

The project automatically identifies:

Highest Sales Category
Highest Profit Category
Highest Sales Sub-Category
Highest Profit Sub-Category
Highest Sales Customer Segment

These results provide a concise summary of the main business findings.

 Simple Predictive Analysis

A simple Linear Regression model is included to demonstrate the basic predictive-analysis workflow.

Target

Sales

Features
Quantity
Discount

The dataset is divided into training and testing sets using an 80/20 split.

The model is evaluated using:

Mean Absolute Error (MAE)
R-squared (R²)

An Actual vs Predicted Sales chart is also created.

Important Limitation

This predictive model is intended as a learning demonstration, not a production-ready sales forecasting system.

Sales can be influenced by many factors that are not included in this simple model, such as product characteristics, customer behaviour, geography, seasonality, pricing, and marketing activity.

 Business Insights

The project demonstrates how analytical results can be translated into business questions and potential actions.

The analysis can help businesses investigate:

Which products generate the most revenue
Which products generate the most profit
Which customer segments are most valuable
Where losses are occurring
Whether discounting may be affecting profitability
Which areas require further investigation

The actual conclusions should be based on the results produced from the dataset.

 Skills Demonstrated
Data Analysis
Data loading
Data inspection
Data quality checking
Missing-value analysis
Duplicate detection
Descriptive statistics
GroupBy and aggregation
Filtering
Business KPI analysis
Data Visualisation
Histograms
Bar charts
Scatter plots
Correlation heatmaps
Python
Pandas
NumPy
Matplotlib
Seaborn
Introductory Machine Learning
Train/test split
Linear Regression
Prediction
MAE
R²
Actual vs Predicted analysis
Business Analysis
KPI interpretation
Product performance
Profitability analysis
Customer segmentation
Identification of loss-making areas
Data-driven recommendations
