# Gym Membership Churn: Survival Analysis

Analysis of customer churn in a gym membership dataset (4,000 customers), combining survival analysis and customer segmentation to identify when and why members leave.

## Key Findings

- **Contract length matters enormously**: churn risk drops from 42% (monthly contracts) to 2% (annual contracts) — an 18x difference
- **Early-warning signal**: customers who churn show a 29% drop in class attendance in their final month compared to their historical average
- **Critical retention window**: Kaplan-Meier survival curve shows the highest churn risk occurs in the first 2-3 months of membership; customers who pass this window tend to stay long-term
- **RFM segmentation**: customers with the lowest RFM scores churn at 53%, compared to just 2% for the highest-scoring segment

## Methodology

- **Data cleaning & exploration** with pandas
- **Survival analysis** using Kaplan-Meier estimation (lifelines library)
- **RFM segmentation** based on recency, frequency, and monetary value of gym usage

## Dataset

Source: [Gym customers features and churn](https://www.kaggle.com/datasets/adrianvinueza/gym-customers-features-and-churn) (Kaggle)

## Tools

Python, pandas, lifelines, matplotlib
