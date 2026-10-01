# Customer Churn Analysis Using Python

## 1. Project Overview

Customer churn refers to the phenomenon where customers discontinue their relationship or subscription with a business over a given period. For subscription-based service models, acquiring new customers is significantly more expensive than retaining existing ones. High churn directly reduces customer lifetime value (CLTV) and recurring revenue, making retention analysis a strategic priority for long-term profitability.

This project conducts an end-to-end quantitative analysis of customer subscription and support interaction data using Python. By analyzing behavioral patterns, demographic attributes, and customer service metrics, the project aims to identify key risk indicators associated with customer drop-off.

By converting raw transactional and support logs into actionable data visualizations and statistical insights, this analysis enables business decision-makers to implement targeted retention strategies, mitigate churn risks, and optimize overall customer satisfaction.

---

## 2. Business Problem

Losing existing customers directly negatively impacts revenue, inflates customer acquisition costs (CAC), and signals potential weaknesses in product offerings or customer support service. Businesses often struggle to proactively identify which customer segments are at risk of churning before they cancel their subscriptions.

This project directly addresses this challenge by analyzing underlying patterns across customer demographics, service plans, billing structures, and support interactions. The core objective is to identify key risk drivers and provide data-backed recommendations to enhance customer retention and protect recurring revenue.

---

## 3. Project Objectives

* Understand overall customer churn and retention rates.
* Analyze customer demographics and subscription behavior across regional and plan segments.
* Identify primary risk drivers and factors associated with subscription cancellations.
* Compare churned versus retained customers across key metrics such as monthly charges, tenure, and customer support history.
* Classify customers into high, medium, and low churn-risk tiers to prioritize retention workflows.
* Generate actionable, data-driven business insights to reduce customer churn.

---

## 4. Dataset

The project utilizes data stored across relational tables in an SQLite database (`customer_churn.db`), encompassing customer profile details, subscription metrics, and service support interactions:

* **Customer Demographics (`db_customer`):** Customer ID, Name, Gender, Date of Birth, State, and Country.
* **Subscription Information (`db_subscription`):** Subscription Start Date, Renewal Date, Cancellation Date, Subscription Type (Paid, Organic, Referral), Plan Type (Basic, Standard, Premium), Contract Type (Monthly, Annual), Monthly Charges, Customer Lifetime Value (CLTV), and Churn Score.
* **Support & Engagement Information (`db_support`):** Complaint Date, Support Escalations, Customer Satisfaction (CSAT) Score, and Complaint Counts.

* **Dataset Size:** 21 unique customer records across merged relational tables.

---

## 5. Tools & Technologies

| Technology | Purpose |
| :--- | :--- |
| Python | Core programming language for data analysis |
| Jupyter Notebook | Interactive development environment for analysis and execution |
| Pandas | Data extraction, manipulation, cleaning, and table merging |
| NumPy | Numerical transformations and conditional array operations |
| Matplotlib | Visualizing monthly churn trends and bar charts |
| Seaborn | Statistical visualization, correlation heatmaps, and pairplots |

---

## 6. Key Analysis / Findings

* **Overall Churn Rate:** 28.57% (Retention Rate: 71.43%).
* **Highest Churn Segment:** Basic Plan Subscribers (60.00% churn rate) and Monthly Contract Holders.
* **Lowest Churn Segment:** Premium Plan Subscribers (14.29% churn rate).
* **Important Churn Factor:** Support Escalations — strong positive correlation of 0.77 between support escalations and customer churn flag.
* **Customer Behavior Insight:** Average Revenue Per User (ARPU) is ₹18.85 / $18.85, with total revenue at risk from churned users totaling 73.94. Average customer tenure across the platform stands at 1,529 days.

---

## 7. Business Insights

### Actual Findings
* **Basic Plan & Monthly Contract Vulnerability:** Customers on Basic plans experience a churn rate of 60.00%, compared to 22.22% on Standard plans and 14.29% on Premium plans. Short-term monthly commitments significantly increase customer attrition risk.
* **Support Escalation as a Primary Churn Driver:** Customer escalations show a strong correlation with churn (0.77). Unresolved support issues and low CSAT scores strongly indicate imminent account cancellation.
* **Revenue Risk Impact:** Revenue lost from churned customers accounts for a significant portion of overall potential monthly revenue (73.94 out of total monthly charges).
drop-off rates.

