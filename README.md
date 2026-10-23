# Telecom Customer Churn Analysis in Excel

![Dashboard](dashboard_screenshot.png)

## Project Overview
Analysis of customer churn in a synthetic telecom dataset (5,030 raw rows, 5,000 after cleaning) to find which customer segments leave most often and what the business can do about it.

Note: the dataset is synthetic and contains no real customer information.

## Tools Used
Excel: Excel Table, Pivot Tables, PivotCharts, Slicers, formulas (COUNTA, COUNTIF, AVERAGE, IF), TRIM, Remove Duplicates

## Data Cleaning
- Removed 30 duplicate rows
- Filled 58 blank TotalCharges with 0 as a placeholder (28 are new customers with tenure 0, 30 are not; TotalCharges is not used in the analysis)
- Fixed extra spaces in City and inconsistent capitalisation in InternetService
- Set number/currency formats and converted the data to an Excel Table
- Converted the data to an Excel Table and added two helper columns (MonthlyCharges_Band, RiskSegment, TenureGroup, ChurnFlag)

## Key Findings
- Overall churn is 32.3% (1,615 of 5,000 customers)
- Month-to-month contracts churn at 50.9%, versus 16.6% (one-year) and 3.8% (two-year)
- Churn is 57.5% in the first 12 months and 3.3% after 60 months
- Customers with 3+ support tickets churn at 42.0%, versus 29.0% for 0-2 tickets
- Fiber optic customers churn at 40.9%, versus 25.1% for DSL
- High-risk segment (month-to-month, fiber optic, tenure 0-11 months): 446 customers, 69.3% churn, 19.1% of all churned customers
- Customers without Tech Support churn at 37.8%, versus 27.2% with it
- Customers paying above ₹70 a month churn at 38-41%, versus 25-28% for ₹70 or less
- Churned customers represent ₹111,097 in monthly charges (₹13.3 lakh a year, assuming none are replaced)
- Gender, partner, dependents, paperless billing and phone service show almost no difference

## Recommendations
- Offer discounts to move month-to-month customers to annual plans
- Build an onboarding programme with check-ins in the first 6 months
- Prioritise resolution for customers with 3+ support tickets
- Target the high-risk segment with onboarding support and annual-plan offers
- Bundle Tech Support and Online Security in the first year
- Review value for higher-priced plans

## Limitations
The data is synthetic, so the patterns show association, not proven cause. KPI cards show overall figures and are not affected by the slicers.

## Files
- `Customer_Churn_Analysis.xlsx`: full workbook (cleaning log, pivots, dashboard)
- `customer_churn_sample.csv`: raw dataset
- `dashboard_screenshot.png`: dashboard preview

Prepared by Birpal Singh | linkedin.com/in/BirpalSingh
