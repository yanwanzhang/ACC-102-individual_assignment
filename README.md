# Financial Ratio Analysis of Four FMCG Companies (2018–2023)
## 1. Problem & User
This project aims to explore how global economic fluctuations and the COVID-19 pandemic impacted the profitability, operational efficiency and financial stability of leading fast-moving consumer goods (FMCG) companies from 2018 to 2023.
It is designed for business school students, beginner investors and industry learners who want to understand corporate financial benchmarking and ratio analysis.
## 2. Data (source + access date + key fields)
-**Data Source**: WRDS Compustat Annual Fundamentals Database
-**Access Date**: 22 April 2026
-**Covered Companies**: Procter & Gamble (PG), Unilever (UL), Coca-Cola (KO), PepsiCo (PEP)
-**Key Fields**: Net Income, Total Equity, Revenue, Total Assets, Liabilities, Inventory, Current Assets & Liabilities
## 3. Methods 
1. Connect to WRDS database and extract annual financial data
2. Data cleaning, filtering and year alignment
3. Calculate core financial ratios: ROE, ROA, Net Profit Margin, Gross Margin, Asset Turnover, Financial Leverage, Debt-to-Equity and Current Ratio
4. Conduct horizontal year-over-year trend analysis and vertical cross-company benchmarking
5. Generate data visualisation charts for clear result comparison
## 4. Key Findings
1.All four FMCG companies showed strong industry resilience during the COVID-19 period (2020–2021). Despite temporary dips in return ratios and margins in 2019, all businesses recovered rapidly and maintained generally solid financial performance across the entire 2018–2023 timeframe.
2.Coca-Cola consistently records the highest gross margin (remaining above 61% for all years), followed by PepsiCo, Procter & Gamble and Unilever, reflecting Coca-Cola’s superior brand pricing power and cost control capability.
3.PepsiCo and Unilever started with the highest ROE and ROA in 2018, but experienced larger volatility and an overall downward trend afterwards. In contrast, Procter & Gamble hit a low point in 2019 and then delivered steady, continuous growth in both ROE and ROA, showing the most stable long-term profitability improvement.
4.PepsiCo maintains the highest financial leverage and debt-to-equity ratio across the period, representing the most aggressive, debt-heavy business model. Procter & Gamble operates with the lowest leverage and gearing level, holding the most conservative and low-risk capital structure of the four firms.
5.Unilever and PepsiCo lead in asset turnover, demonstrating stronger asset utilisation and core operational efficiency. Coca-Cola holds the highest current ratio with the best short-term liquidity position, and all four companies maintained healthy overall solvency throughout the analysis period.
## 5. How to run
1. Install required Python libraries: `wrds`, `pandas`, `matplotlib`
2. Log in with valid WRDS account credentials
3. Run the `notebook.ipynb` file step by step
4. Full dataset and charts will be generated automatically
## 6. Product link / Demo
GitHub Repository:
Project Demo Video：
## 7. Limitations & next steps
### Limitations
1.This analysis only uses annual consolidated data, without quarterly detailed performance insight.
2.Only 4 companies are included, lacking wider industry peer benchmark comparison.
3.Macroeconomic factors like inflation and exchange rate are not integrated into the model.
### Next Steps
1.Expand the dataset to include more global FMCG competitors.
2.Introduce DuPont ROE decomposition for deeper driver analysis.
3.Add regression modelling to quantify external economic impact.
