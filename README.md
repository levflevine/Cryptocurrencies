# Cryptocurrencies

## Overview of the Analysis

### Purpose

Create a report that includes what cryptocurrencies are on the trading market and how they could be grouped to create a classification system for this new investment.

### Approach

The cryptocyrrency data is not ideal and will need to be processed to fit the machine learning models. Since there is no known output for what we are looking for,   unsupervised learning will be used. To group the cryptocurrencies, we will use a clustering algorithm. Once the clustering is performed, data visualizations will be used to share the findings.

### Deliverables: 

1. Preprocessing the Data for PCA
2. Reducing Data Dimensions Using PCA
3. Clustering Cryptocurrencies Using K-means
4. Visualizing Cryptocurrencies Results 

### Tools and Data Sources

#### Tools

- Python Scripts
- Pandas Library
- Sklearn Library
- hvPlot Library
- Plotly Library

#### Data Sources

- [Crypto_Curency_Dataset](https://min-api.cryptocompare.com/data/all/coinlist)

## Results

### Data Cleaning

Cleaned Crypto Currency DataFrame

![Cleaned_df](/Resources/crypto_clean_df.png)

### Data Encoding with get_dummies (converting text data into numeric format)

Encoded Crypto Currency Data:

![Encoded_df](/Resources/get_dummies.png)

### Data Scaling with Standard_Scaler (standardizing the features to distributionm with St. Dev = 1 and Mean = 0)

Scaled Crypto Currency Data:

![Scaler](/Resources/standard_scaler.png)

### Reducing Data Dimensions Using Principal Component Analysis (PCA) to 3 Principal Components (Features)

Reduced-Dimention Feature Data:

![PCA](/Resources/pca.png)

### Creating an Elbow Curve to Find the Best Value for K before We Can Apply K-Means Algo

Elbow Curve:

![Elbow_Curve](/Resources/elbow_curve.png)

### Running K-Means with k=4

Class Prediction:

![Encoded_df](/Resources/k_means.png)

### Concatenating Two DataFrames (Crypto Currency Data & Reduced Featureset Data) into a New DataFrame and Adding Predicted Clusters

Clustered Data:

![Clastered_Data](/Resources/concat_class.png)

### Creating a 3D-Scatter with the PCA Data and the Clusters

3d Scatter Plot of the Crypto Currency Clusters:

![3d_Scatter_Plot](/Resources/3d_scatter.png)

### Creating an Interactive Table with Tradable Cryptocurrencies

Crypto Currency Table:

![Table](/Resources/table.png)

### Counting Tradable Cryptocurrencies

![Number](/Resources/number_crypto.png)

### Scaling the Tradable Cryptocurrencies Data with MinMaxScaler (to Standardize the 'TotalCoinSupply' and 'TotalCoinsMined')

Scaled Data:

![Table](/Resources/min_max_scaler.png)

### Creating a New DataFrame that has the Scaled Data with the Clustered_df DataFrame Index

Scaled DataFrame:

![Scaled_DataFrame](/Resources/scaled_df.png)

### Creating a hvplot.scatter plot using x="TotalCoinsMined" and y="TotalCoinSupply"

Scaled Scatter Plot:

![Scatter_Plot](/Resources/scaled_df_plot.png)

## Summary

The project resulted in 

- Visualizing 4 distinct groups of traded Crypto currencies
- Creating a table with the details on all the currently tradable cryptocurrencies 
