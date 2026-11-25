# Banking-Strategic-Insights-Tableau
Banking Strategic Insights Dashboard built in Tableau using MySQL (CodeBasics Resume Project Challenge 11)
An interactive Tableau dashboard that gives a bank's Product Strategy Team insights into customer spending, income and income utilization. Built for CodeBasics Resume Project Challenge 11.

**Live dashboard:** https://public.tableau.com/app/profile/priyanka.singh1212/viz/Banking_Strategic_Dashboard/HomePage

## Business Problem
The Product Strategy Team wants to understand who the credit card customers are, how they spend, and how much of their income they use, so they can design better products and offers.

## Dataset
- `dim_customers` : 4,000 customers (age group, city, occupation, gender, marital status, average income)
- `fact_spends` : 8,64,000 spend records (month, category, payment type, spend) for May to October

## Tools Used
- MySQL (data loading with LOAD DATA LOCAL INFILE)
- Tableau (relationships, calculated fields, dashboards, filters, maps)

## Dashboard Pages
1. Home Page (navigation)
2. Demographic Analysis
3. Spending Analysis 1
4. Spending Analysis 2
5. Avg Income Util Analysis
6. Detailed Analysis

## Key Calculations
- Avg Spending = SUM(Spend) / COUNTD(Month)
- Avg Income Utilization = Avg Spending / SUM(Avg Income)
- Customer Segmentation: Upper Class (income >= 80,000), Middle Class (>= 45,000), Lower Class (below 45,000)

## Key Insights
- 4,000 customers; average monthly spend is 88.48M against 206.63M average income, an overall income utilization of 42.82%.
- Bills is the top spending category (17.49M), followed by Groceries and Electronics.
- Credit Card is the most used payment mode (36.05M spend).
- Salaried IT Employees spend the most (40.62M) and also use the highest share of income (51.04%).
- The 25-34 age group spends the most (33.89M); spending peaks in September (115.93M).
- Male customers use 44.39% of income versus 39.92% for female customers.

## Author
Priyanka Singh
