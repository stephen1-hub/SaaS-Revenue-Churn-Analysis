# SaaS Customer Churn and Profitability Analysis

## Project Overview

This project analyzes customer churn patterns and profitability for a cloud-based SaaS platform. The goal is to understand the factors that influence customer churn and identify which customer segments generate the most long-term value.

Using Python and data analysis techniques, the project explores customer behavior across different subscription plans, billing cycles, industries, and company sizes.

The insights from this analysis help inform strategies to improve customer retention and increase profitability.

---

# Dataset Description

The dataset contains subscription data for customers over a four-year period.

Key variables include:

- customer_id – Unique customer identifier
- plan – Subscription plan (Starter, Professional, Business, Enterprise)
- billing_cycle – Monthly or Annual subscription
- industry – Customer industry
- company_size – Number of employees
- seats – Number of users
- monthly_revenue – Monthly subscription revenue
- acquisition_channel – Marketing channel used to acquire the customer
- signup_date – Date customer joined
- churned – Whether the customer churned (1) or stayed (0)
- churn_reason – Reason for churn
- support_tickets_12mo – Number of support requests
- nps_score – Customer satisfaction score
- feature_usage_pct – Percentage of platform features used
- upgraded – Whether the customer upgraded plans

---

# Project Objectives

The analysis focuses on answering the following questions:

1. What is the overall customer churn rate?
2. How does churn vary by subscription plan and billing cycle?
3. What factors are associated with customer churn?
4. Which industries and company sizes have the highest churn rates?
5. What are the main reasons customers churn?
6. What is the Customer Lifetime Value (CLV) by plan?
7. Which plans are the most and least profitable?

---

# Tools and Technologies

- Python
- Pandas
- NumPy
- Jupyter Notebook
- Data Visualization (Matplotlib / Seaborn)

---

# Data Cleaning

The dataset was checked for missing values and inconsistencies.

Missing values in churn-related fields were handled appropriately:
- Customers who did not churn had null values for churn date and churn reason.
- These were left unchanged because they represent active customers.

Additional calculated fields were created including:
- churn_rate
- estimated_customer_lifetime
- customer_lifetime_value (CLV)
- CLV to CAC ratio

---

# Key Findings

## Overall Churn Rate

The overall churn rate across the dataset is:

**52.17%**

This means that more than half of the customers left the platform during the four-year period.

---

# Churn by Subscription Plan

| Plan | Churn Rate |
|-----|-----|
| Starter | 70.5% |
| Professional | 48.0% |
| Business | 41.3% |
| Enterprise | 22.0% |

Starter customers churn the most, while Enterprise customers have the strongest retention.

---

# Churn by Billing Cycle

| Billing Cycle | Churn Rate |
|-----|-----|
| Monthly | 60.5% |
| Annual | 40.3% |

Customers with monthly subscriptions churn significantly more than those on annual plans.

---

# Churn by Industry

Highest churn industries:
- Real Estate
- Finance
- Retail

Lowest churn industries:
- Education
- Media
- Technology

---

# Churn by Company Size

| Company Size | Churn Rate |
|-----|-----|
| 500+ | 63.2% |
| 1–10 | 56.7% |
| 201–500 | 53.4% |
| 11–50 | 52.8% |
| 51–200 | 42.6% |

Mid-sized companies (51–200 employees) demonstrate the strongest retention.

---

# Feature Usage and Churn

Product engagement strongly correlates with retention.

| Customer Type | Avg Feature Usage |
|-----|-----|
| Active Customers | 55% |
| Churned Customers | 27% |

Customers who use fewer product features are significantly more likely to churn.

---

# Customer Lifetime Value (CLV) Analysis

| Plan | CLV ($) | CAC ($) | CLV:CAC |
|-----|-----|-----|-----|
| Enterprise | 13,568 | 178 | 76:1 |
| Business | 3,160 | 210 | 15:1 |
| Professional | 1,036 | 203 | 5:1 |
| Starter | 306 | 184 | 1.66:1 |

Enterprise and Business customers generate the highest lifetime value, while Starter customers produce the lowest return due to high churn.

---

# Key Business Insights

- Monthly customers churn significantly more than annual customers.
- Lower-tier plans experience the highest churn.
- Low product engagement is a strong predictor of churn.
- Mid-sized companies represent the most stable customer segment.
- Enterprise customers generate the highest profitability.

---

# Strategic Recommendations

Based on the analysis:

1. Encourage annual subscriptions to reduce churn.
2. Improve onboarding to increase feature adoption.
3. Focus marketing on Business and Enterprise customers.
4. Improve product features and support to reduce churn.
5. Implement strategies to convert Starter users to higher plans.

---

# Project Structure

