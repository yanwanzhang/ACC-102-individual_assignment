# FMCG Profitability Analysis: How Discounts and Cost Structure Affect Profit Margin

**Main notebook:** `success.ipynb`  
**Demo video (1–3 minutes):** (demo video link)

## 1. Problem & User
This project investigates how discount strategy, promotion type, sales channel, and cost structure influence profit margin in an FMCG dataset. The analysis is designed for beginner investors, business students, and FMCG industry analysts who want a simple but evidence-based understanding of the key drivers of profitability.

## 2. Data
- **Source:** Kaggle – FMCG Sales & Profit Dataset (2023–2025)
- **Dataset link:** https://www.kaggle.com/datasets/atharvasoundankar/fmcg-sales-marketing-and-profit-data
- **Dataset file used:** `fmcg_sales_marketing_profitability_2023_2025.csv`  
- **Access date:** 23 April 2026  

### Key fields used
- `Discount_Pct`
- `Profit_Margin_Pct`
- `Promotion_Type`
- `Sales_Channel`
- `COGS_USD`
- `Logistics_Cost_USD`
- `Net_Revenue_USD`
- `Year`
- `Product_Category`

### Derived variable
A new variable called `Total_Cost_Ratio` was created to capture the combined cost burden relative to revenue:

`Total_Cost_Ratio = (COGS_USD + Logistics_Cost_USD) / Net_Revenue_USD`

This variable is used to examine how cost structure is associated with profit margin.

## 3. Methods
This project follows a clear Python-based analytical workflow from raw data to business insight.

### Step 1: Data loading
- Imported the CSV dataset using `pandas`
- Inspected the dataset structure, column names, and summary statistics

### Step 2: Data cleaning
- Converted key variables into numeric format using safe conversion
- Handled missing and invalid values
- Excluded rows where `Net_Revenue_USD` was zero before calculating ratios
- Used a cleaned dataset for the main analysis

### Step 3: Feature engineering
- Created `Total_Cost_Ratio`
- Prepared grouped summaries by promotion type, sales channel, year, and product category

### Step 4: Descriptive analysis
The notebook examines:
- the relationship between `Discount_Pct` and `Profit_Margin_Pct`
- average profit margin by `Promotion_Type`
- average discount by `Sales_Channel`
- the distribution of `Total_Cost_Ratio`
- yearly changes in average profit margin
- average profit margin across product categories
- the relationship between `Total_Cost_Ratio` and `Profit_Margin_Pct`

### Step 5: Visualisation
The analysis uses `matplotlib` and `seaborn` to create:
- scatter plots
- boxplots
- bar charts
- histograms
- line charts

These visualisations are used to support interpretation and communicate the results clearly.

### Step 6: Predictive modelling
A Random Forest regression model is used to predict `Profit_Margin_Pct` and identify the most important variables affecting profitability.

### Step 7: Conclusion
The project combines descriptive analysis and machine learning evidence to answer the main business question: which factors are most strongly associated with FMCG profit margin?

## 4. Key Findings
- There is a negative relationship between discount percentage and profit margin, suggesting that heavier discounting is generally associated with lower profitability.
- Profit margin differs across promotion types, indicating that not all promotional strategies are equally effective.
- Average discount levels vary across sales channels, showing that pricing strategy is not the same in every channel.
- `Total_Cost_Ratio` is an important predictor of profit margin, highlighting the role of cost control in FMCG performance.
- Profitability also varies across years and product categories, suggesting that margin outcomes depend on both time-related and product-related factors.

## 5. How to run
1. Download or clone this repository.
2. Make sure Python 3 is installed.
3. Install the required libraries:
   ```bash
   pip install -r requirements.txt
   ```
4.Place the dataset file fmcg_sales_marketing_profitability_2023_2025.csv in the same folder as the notebook.
5.Open success.ipynb in Jupyter Notebook and run all cells.

## 6. Limitations & Next Steps
This project has several limitations. First, the analysis is based on one dataset, so the findings may not fully represent the entire FMCG industry. Second, the project mainly identifies patterns, correlations, and predictive importance, but these do not prove causality. Third, some potentially useful business variables, such as region, customer segment, seasonality, or brand-level information, are not included in the dataset.

Future improvements could include:
- adding more business variables for richer analysis
- comparing Random Forest with simpler models such as linear regression
- improving feature engineering and model evaluation
- building a more interactive dashboard for users
- testing whether the same relationships hold in other FMCG datasets
