# Developers_Hub-Customer_Segmentation-Internship-task-
Data Science &amp;amp; Analytics internship tasks completed for the DevelopersHub Corporation internship program (June-15July 2026).

# Customer Segmentation Using Unsupervised Learning

## Project Objective
The goal of this project is to analyze customer demographic and purchasing data to identify distinct customer segments based on their spending habits and income levels. By applying clustering algorithms, we aim to deliver actionable insights and data-driven marketing strategies tailored to each specific customer profile.

## Dataset Description
The analysis is performed on the **Mall Customers Dataset**, which contains structural demographic and behavioral insights of retail customers:
*   **CustomerID:** Unique identifier for each customer.
*   **Gender:** Gender of the customer (Male/Female).
*   **Age:** Age of the customer.
*   **Annual Income (k$):** Annual income of the customer in thousands of dollars.
*   **Spending Score (1-100):** Score assigned by the mall based on customer behavior and spending history.

## Technical Approach & Workflow
1.  **Exploratory Data Analysis (EDA):** Visualized distribution trends of numerical attributes (Age, Income, Spending Score) using histograms and analyzed internal feature correlations with scatter plots.
2.  **Data Preprocessing:** Handled continuous variables and applied `StandardScaler` to normalize features, ensuring equal weighting during the clustering process.
3.  **Optimal Cluster Identification:** Used the **Elbow Method** to calculate the Within-Cluster Sum of Squares (WCSS) across varying cluster numbers, successfully identifying $K = 5$ as the optimal number of segments.
4.  **Model Training:** Fitted a `KMeans` clustering algorithm on the scaled feature space using `k-means++` initialization for stable convergence.
5.  **Dimensionality Reduction & Visualization:** Implemented Principal Component Analysis (PCA) to structure and visualize the multidimensional boundaries clearly in a 2D plane.

## Key Findings & Suggested Marketing Strategies

Based on our model, the customer base was segmented into 5 distinct groups:

*   **Cluster 0 (High Income, Low Spending):** *Targeted Luxury Offers.* These customers have high purchasing power but low engagement. Focus on exclusive premium collections, private previews, and VIP product alerts.
*   **Cluster 1 (Low Income, High Spending):** *Budget-Friendly Triggers.* Active shoppers with constrained budgets. Highly responsive to flash sales, discount coupons, and "Buy One Get One" campaigns.
*   **Cluster 2 (High Income, High Spending):** *VIP Loyalty Program.* The most valuable segment. Retain them through premium subscription models, personalized rewards, and dedicated customer support.
*   **Cluster 3 (Low Income, Low Spending):** *Value Packs & Essentials.* Price-sensitive and low-frequency shoppers. Focus on high-utility bundle offers and daily essential promotions.
*   **Cluster 4 (Average Income, Average Spending):** *Engagement Campaigns.* Standard mainstream consumers. Boost their conversion rates via seasonal discounts, holiday sales, and mid-tier loyalty perks.

## Tools & Libraries Used
*   **Language:** Python
*   **Environment:** Google Colab
*   **Libraries:** `pandas`, `numpy`, `scikit-learn`, `matplotlib`, `seaborn`

---
*This repository is part of the Advanced Data Science Internship track at Developers Hub Corporation.*

