# SME Customer Lifetime Value (CLV) Segmentation

## Business Context
Retention resources are limited, and not all customers contribute equally to long-term revenue.
Understanding which customers are most valuable allows organizations to prioritize retention and pricing strategies.

## Objective
This project estimates **relative customer lifetime value (CLV)** and segments SME customers into value-based groups to support targeted decision-making.

## CLV Definition (Proxy-Based)
Due to the absence of future transaction data, CLV is estimated using a proxy-based approach:

CLV Score = MonthlyCharges × Tenure × Retention Factor

Where:
- MonthlyCharges represents revenue intensity
- Tenure captures relationship length and stability
- Retention Factor discounts churned customers

This approach enables **comparative value segmentation**, not precise financial forecasting.

## Scope
- Focus on relative CLV ranking and segmentation
- Emphasis on interpretability and business relevance
- Designed to complement churn diagnostics

## Analysis Overview

The project follows an end-to-end customer analytics workflow:

1. Feature engineering to construct a proxy-based CLV score
2. Preparation of behavioral and value-based features for segmentation
3. Customer segmentation using KMeans clustering
4. Profiling and interpretation of customer segments
5. Translation of segments into actionable business strategies

## Key Outcomes

- Identified distinct customer segments based on lifetime value and engagement
- Highlighted high-value customers requiring retention focus
- Identified growth segments suitable for upsell and bundling strategies
- Flagged low-value segments for cost-aware engagement decisions

The final output supports data-driven prioritization of retention, pricing, and customer investment strategies.

## Tools & Techniques
Python, Pandas, Scikit-learn, KMeans Clustering, Jupyter Notebook

## Repository Structure
- notebooks/ — CLV feature engineering, segmentation, and strategy
- data/ — Raw input dataset
- README.md — Project overview and outcomes

