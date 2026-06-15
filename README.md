# Mall Customer Segmentation using K-Means Clustering

## Project Overview

Customer segmentation is a common business strategy used to group customers based on shared characteristics and purchasing behavior. Identifying customer segments enables businesses to design targeted marketing campaigns, improve customer retention, and optimize resource allocation.

In this project, K-Means Clustering was applied to the Mall Customers dataset to discover distinct customer groups based on:

- Age
- Annual Income (k$)
- Spending Score (1–100)

The project follows a complete machine learning workflow including data exploration, preprocessing, clustering, cluster evaluation, visualization, and business interpretation.

---

## Dataset

The dataset contains customer information collected by a shopping mall.

### Features

| Feature | Description |
|----------|-------------|
| CustomerID | Unique customer identifier |
| Gender | Male/Female |
| Age | Customer age |
| Annual Income (k$) | Annual income in thousand dollars |
| Spending Score (1-100) | Spending behavior score assigned by the mall |

Dataset Size:

- 200 Records
- 5 Features

---

## Project Workflow

### 1. Exploratory Data Analysis (EDA)

The dataset was inspected for:

- Missing values
- Duplicate records
- Data types
- Statistical summaries
- Feature distributions

Visualizations included:

- Histograms
- Pairplots
- Correlation analysis

---

### 2. Data Preprocessing

The following preprocessing steps were performed:

- Gender encoding
- Feature selection
- Standardization using StandardScaler

Feature scaling was required because K-Means is distance-based and sensitive to feature magnitude.

---

### 3. Optimal Cluster Selection

The optimal number of clusters was determined using:

- Elbow Method
- Silhouette Score

Five clusters were selected as they provided a good balance between cluster compactness and separation.

---

### 4. Customer Segmentation

K-Means clustering was applied using:

- Age
- Annual Income
- Spending Score

The resulting clusters revealed meaningful customer segments with distinct demographic and spending characteristics.

---

### 5. PCA Visualization

Principal Component Analysis (PCA) was used to reduce the dimensionality of the dataset and visualize clusters in two dimensions.

This provided an intuitive representation of customer groups while preserving most of the information contained in the original feature space.

---

## Cluster Summary

### Cluster 0 – Middle-Aged Low-Spending Customers

- Moderate age
- Low income
- Low spending

### Cluster 1 – Average Customers

- Average age
- Average income
- Average spending

### Cluster 2 – Young High-Value Customers

- Younger customers
- High income
- High spending

### Cluster 3 – High-Income Low-Spending Customers

- High income
- Low spending

### Cluster 4 – Young Enthusiastic Shoppers

- Younger customers
- Lower income
- High spending

---

## Key Business Insights

### Most Valuable Customers

Cluster 2 represents high-income and high-spending customers. These customers are ideal targets for:

- Loyalty programs
- Premium products
- Personalized marketing campaigns

### Growth Opportunity

Cluster 3 contains customers with high purchasing power but relatively low spending behavior. Targeted promotions may encourage increased engagement and spending.

### Budget-Conscious Customers

Cluster 0 customers have lower income and spending levels and may respond well to discounts and promotional offers.

---

## Technologies Used

- Python
- Pandas
- Matplotlib
- Seaborn
- Scikit-Learn

---

## Evaluation Metric

The clustering performance was evaluated using the Silhouette Score.

- 2-feature model (Income + Spending Score): **55.39%**
- 3-feature model (Age + Income + Spending Score): **~44%**

Although the 2-feature model achieved a higher silhouette score, the 3-feature model was selected because it provides richer customer profiles by incorporating age information, resulting in more actionable business insights.

---

## Results

- Successfully segmented customers into five meaningful groups.
- Identified high-value customer segments.
- Visualized cluster separation using PCA.
- Generated business recommendations based on customer behavior.

---

## Future Improvements

Potential enhancements include:

- Comparing K-Means with Agglomerative Clustering
- Testing DBSCAN on larger datasets
- Building customer recommendation systems
- Deploying the project as an interactive dashboard

---

## Author

Shivansh Pandey

Machine Learning & Data Science