Retail Sales & Performance Analysis

Exploratory data analysis and predictive modeling on the Global Superstore dataset — a retail transactions log covering four years of orders across seven markets (US, EU, LATAM, Africa, APAC, EMEA, Canada).

Dataset

superstore.csv — 51,290 order line items, 27 columns, spanning 2011–2014. No missing values or duplicate rows.

Key fields: Category, Sub.Category, Region, Market, Segment, Sales, Profit, Quantity, Discount, Shipping.Cost, Order.Date, Ship.Date, Order.Priority.

What's in the notebook

Retail_Sales___Performance_Analysis.ipynb walks through a full analysis pipeline:

1. Data quality checks

Shape, dtypes, missing values, and duplicate detection

2. Exploratory analysis

Distributions of Sales, Quantity, Discount, and Profit
Correlation matrix and pairplot across numerical variables

3. Category & sub-category performance

Average Sales and Profit grouped by Category and Sub.Category
Example finding: Technology leads in both average sales (~$468) and average profit (~$65) per order, followed by Furniture, with Office Supplies trailing on both metrics despite likely higher order volume

4. Predictive modeling

Features: Quantity, Discount, Category, Sub.Category, Segment (one-hot encoded)
Target: Sales
Models compared: Linear Regression vs Decision Tree Regressor
Evaluation via MAE, MSE, and R²
Getting started
bash
pip install pandas numpy matplotlib seaborn scikit-learn

Open the notebook in Jupyter or Google Colab and run all cells. The first cell uses Colab's file upload widget — if running locally, replace it with:

