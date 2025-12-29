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
