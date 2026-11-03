# 📉 Customer Retention & Churn Analysis | Power BI Dashboard

An interactive Power BI dashboard that analyzes why telecom customers leave, which segments are most at risk, and how much revenue is on the line, followed by data-driven retention recommendations.

Dashboard Preview

## 📌 Table of Contents
- Business Problem
- Dataset
- Tools & Skills
- Dashboard Overview
- Key Insights
- Strategic Recommendations

## 🎯 Business Problem

A telecom company is losing customers and revenue to churn. Leadership needs to know:

How big is the churn problem, and what does it cost?
Which customer segments and service features are driving churn?
What actions can reduce churn and protect recurring revenue?

## 🗂 Dataset
Source: IBM Telco Customer Churn dataset (WA_Fn-UseC_-Telco-Customer-Churn)
Size: ~7,043 customers
Features include: contract type, tenure, internet service, tech support, payment method, monthly and total charges, demographics (senior citizen, partner, dependents), and a churn flag.

## 🛠 Tools & Skills
- Power BI Desktop for data modeling and dashboard design
- DAX for measures (churn rate, monthly charge at risk, tenure brackets, and more)
- Power Query for data cleaning and transformation
- Skills demonstrated: KPI design, segmentation analysis, data storytelling, business recommendations

## 📊 Dashboard Overview
| KPI |	Value
|---|---|
| Customers |	~7K
| Churn Rate |	26.54%
| Average Tenure |	32.37 months
| Monthly Charge (total) |	456.12K
| Monthly Charge at Risk |	139.13K
| Total Charge |	16.06M
| Avg Total Charge at Risk |	1.53K

Visuals included: churn by contract, tech support, dependents, partner, senior citizen, payment method, monthly charge bins, internet service vs. tenure, and tenure bracket.

## 🔍 Key Insights
1. The overall cost of churn: About 26.54% of customers (1,858) have churned, putting 139.13K in monthly revenue at risk (~$1.67M annualized). Churners pay more than average ($75 vs. $65 per month), so revenue loss is outpacing customer loss.


2. Contract type is the strongest churn driver: Month-to-month customers churn at 42.71%, roughly 15x the rate of two-year customers (2.83%), and account for 75.18% of all churners. Longer contracts clearly improve retention, though part of that effect may be lock-in rather than true loyalty.

3. Tech support reduces churn: Customers without tech support churn at 41.64%, about 2.7x the rate of those with it (15.17%), excluding customers with no internet service. Unresolved technical issues likely push customers out the door.

4. Fiber optic customers churn at about twice the DSL rate: Fiber optic customers churn at 41.89%, about 2x the rate of DSL customers. Churned fiber customers had an average tenure of 20.2 months vs. 14.1 months for DSL, so these are established, higher-paying customers leaving, which points to a product or pricing problem rather than an onboarding problem.

5. Churn peaks in higher-priced plans: Churn is highest in the ~$68-$100 monthly charge range (up to ~39%), where fiber plans typically sit, and lowest in the cheapest bin (~9%). The pattern is not uniform across price points, so price is a likely contributor rather than the sole cause.

6. Customers with fewer household ties churn more:
 - Senior citizens churn at roughly 2x the rate of non-seniors.
 - Customers without dependents churn at 31.3% vs. 15.5% for those with dependents.
 - Customers with a partner churn less (19.66%).

The highest-risk profile is a single senior customer living alone.

7. Manual payers churn about twice as much as automatic payers: Customers paying by electronic or mailed check churn at roughly 2x the rate of those on automatic payments (bank transfer or credit card). Credit card payers are among the most loyal at 15.24%. Automatic payments may reduce churn by removing the monthly decision point.


## 💡 Strategic Recommendations
| Problem	Recommendation |	Expected Impact
|---|---|
| 1.	75% of churners are on month-to-month contracts	Offer discounts or perks (free upgrade, bill credit) for moving to 12- or 24-month contracts, targeted at month-to-month customers in their first year	Lower churn in the largest at-risk segment | Lower churn in the largest at-risk segment
| 2.	No tech support = 2.7x higher churn	Bundle tech support free for the first 3-6 months, especially with fiber plans, and add proactive outreach after service issues	Fewer unresolved issues and lower churn | Fewer unresolved issues and lower churn
| 3.	Fiber customers churn at 2x DSL	Audit fiber pricing against competitors, run satisfaction surveys on reliability and speed, and add loyalty pricing at the 12-24 month mark, when fiber churn occurs	Protect high-value customers | Protect high-value customers
| 4.	Manual payers churn 2x more	Offer a small credit or discount for enrolling in autopay, starting with electronic check users	Higher retention through lower billing friction | Higher retention through lower billing friction
| 5.	Single seniors are the highest-risk profile	Create a senior-friendly plan with simplified billing and a dedicated support line, plus household or family bundles	Reduce churn in a vulnerable segment | Reduce churn in a vulnerable segment
| 6.	Churn is only visible after it happens	Build a churn-risk score from contract, tenure, tech support, and payment method, and trigger retention outreach for high-risk accounts	Shift from reactive to proactive retention | Shift from reactive to proactive retention

Illustrative impact: each 1-percentage-point reduction in churn is worth about $5.2K in monthly revenue (~$63K annually). A 5-point reduction would protect roughly $315K per year.

<img width="666" height="332" alt="Screenshot 2025-12-29 184238" src="https://github.com/user-attachments/assets/8952ce95-6a25-47ca-9d8b-4059c45154c4" />



