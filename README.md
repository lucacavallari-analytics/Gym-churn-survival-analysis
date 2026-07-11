# Gym Membership Churn: Survival Analysis

Analysis of customer churn in a gym membership dataset (4,000 customers), combining survival analysis and customer segmentation to identify when and why members leave.

## Key Findings

- **Contract length matters enormously**: churn risk drops from 42% (monthly contracts) to 2% (annual contracts) an 18x difference
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


## Power BI Dashboard

An interactive dashboard built in Power BI on the same dataset, summarising the churn analysis for a business audience.

![Dashboard](Dashboard%20Gym_Churn_Analysis.png)

**What it shows:**
- KPI overview: overall churn rate, total members, average age and average lifetime
- Churn rate by contract length: monthly contracts churn far more than annual ones (42% vs 2%)
- Class attendance drop: members who leave attend fewer classes in their final month than their historical average
- Churn risk over tenure: risk is highest in the first months, then drops sharply for members who pass that window
- A gender slicer for interactive filtering across all visuals
