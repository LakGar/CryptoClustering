# Crypto Clustering

## Overview
This project applies **unsupervised learning** techniques to analyze cryptocurrency market data. Using **K-Means clustering**, the goal is to determine if cryptocurrencies are affected by 24-hour or 7-day price changes.

## Steps
1. **Load and Preprocess the Data**
   - Read `crypto_market_data.csv` into a Pandas DataFrame.
   - Normalize the data using `StandardScaler()`.

2. **Find the Best k Value (Elbow Method)**
   - Use the elbow method to determine the optimal number of clusters.
   - Plot the inertia values for k-values from 1 to 11.

3. **Cluster Cryptocurrencies Using K-Means**
   - Fit the K-Means model with the best k-value.
   - Assign cluster labels to cryptocurrencies.
   - Visualize clusters using a scatter plot.

4. **Optimize Clusters with PCA**
   - Reduce the dataset to **three principal components** using **PCA**.
   - Determine the explained variance of the PCA transformation.

5. **Find the Best k Value Using PCA Data**
   - Repeat the elbow method on the PCA-reduced dataset.
   - Compare the best k-values found before and after PCA.

6. **Cluster Cryptocurrencies Using PCA Data**
   - Fit K-Means to the PCA dataset.
   - Assign cluster labels and visualize the results.

7. **Compare Results**
   - Compare clustering results before and after PCA.
   - Analyze the impact of using fewer features in K-Means.

## Results
- **Best k-value (original dataset):** *Determined using elbow method*  
- **Best k-value (PCA dataset):** *Compared with original dataset*  
- **Total explained variance from PCA:** *Reported in analysis*  
- **Cluster visualizations** comparing original vs. PCA-based clustering.

## Files
- `Crypto_Clustering.ipynb` - Jupyter Notebook with the full analysis.
- `crypto_market_data.csv` - Cryptocurrency market data.
- `README.md` - Project documentation.

## Tools Used
- **Python**
- **Pandas & Scikit-Learn** (Data preprocessing, K-Means, PCA)
- **hvPlot & Matplotlib** (Data visualization)

## Submission
- All files are uploaded to the **CryptoClustering** GitHub repository.
