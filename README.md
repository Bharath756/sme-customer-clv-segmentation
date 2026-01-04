# SME Customer Lifetime Value (CLV) Segmentation

## 1. Business Problem
Retention resources are limited, and not all customers contribute equally to long-term revenue.
Understanding which customers are most valuable allows organizations to prioritize retention and pricing strategies.

This project estimates **relative customer lifetime value (CLV)** and segments SME customers into value-based groups to support targeted decision-making.

## 2. Dataset Overview
(Dataset overview intentionally kept high-level. Data is anonymized and structured to reflect realistic SME scenarios.)

## 3. Approach & Methodology
### CLV Definition (Proxy-Based)
Due to the absence of future transaction data, CLV is estimated using a proxy-based approach:

**CLV Score = MonthlyCharges × Tenure × Retention Factor**

Where:
- MonthlyCharges represents revenue intensity  
- Tenure captures relationship length and stability  
- Retention Factor discounts churned customers  

This approach supports **comparative value segmentation**, not precise financial forecasting.

### Scope
- Focus on relative CLV ranking and segmentation  
- Emphasis on interpretability and business relevance  
- Designed to complement churn diagnostics  

### Analysis Overview
1. Feature engineering to construct a proxy-based CLV score  
2. Preparation of behavioral and value-based features for segmentation  
3. Customer segmentation using KMeans clustering  
4. Profiling and interpretation of customer segments  
5. Translation of segments into actionable business strategies  

## 4. Notebook Walkthrough
- `notebooks/01_clv_feature_engineering.ipynb` — CLV proxy construction, feature engineering, and segmentation preparation

## 5. Key Insights
- Identified distinct customer segments based on lifetime value and engagement  
- Highlighted high-value customers requiring retention focus  
- Identified growth segments suitable for upsell and bundling strategies  
- Flagged low-value segments for cost-aware engagement decisions  

## 6. Tech Stack
Python, Pandas, Scikit-learn, KMeans Clustering, Jupyter Notebook

## 7. Next Improvements
- Add probabilistic CLV estimation when future transaction data is available  
- Integrate CLV segments with churn risk scoring  
- Deploy segment-level dashboards for business teams  
