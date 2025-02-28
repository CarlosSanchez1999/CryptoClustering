# Crypto Clustering

## Overview

This project explores clustering techniques on cryptocurrency market data using **K-Means** and **Principal Component Analysis (PCA)**. The objective is to segment cryptocurrencies based on their price change percentages over different timeframes and analyze how dimensionality reduction affects clustering results.

## Technologies Used

- **Python**
- **pandas** for data manipulation
- **hvPlot** for interactive visualizations
- **scikit-learn** for clustering and PCA
- **StandardScaler** for feature scaling
- **Jupyter Notebook**

## Data Source

The dataset used is **crypto_market_data.csv**, which contains cryptocurrency price change percentages over multiple timeframes.

## Installation

1. Clone this repository:
   ```sh
   git clone https://github.com/yourusername/crypto-clustering.git
   ```
2. Navigate to the project directory:
   ```sh
   cd crypto-clustering
   ```
3. Install the required dependencies:
   ```sh
   pip install -r requirements.txt
   ```
4. Launch Jupyter Notebook:
   ```sh
   jupyter notebook
   ```

## Project Steps

1. **Load and Explore the Data**
   - Read the dataset using pandas
   - Generate summary statistics
   - Visualize price trends using hvPlot

2. **Prepare the Data**
   - Normalize the features using StandardScaler
   - Create a new DataFrame with the scaled data

3. **K-Means Clustering**
   - Find the optimal number of clusters using the Elbow Method
   - Perform clustering on the original dataset
   - Visualize the results in a scatter plot

4. **Dimensionality Reduction with PCA**
   - Reduce data to two principal components
   - Re-run K-Means on the PCA-transformed data
   - Compare clustering results before and after PCA

5. **Results Analysis**
   - Compare how feature reduction affects clustering
   - Discuss trade-offs between using original features vs. PCA-transformed features

## Usage

Run the Jupyter Notebook **Crypto_Clustering.ipynb** to execute the entire clustering workflow. The outputs will include:

- Summary statistics of the data
- Elbow curve plots to determine the optimal K for K-Means
- Scatter plots comparing clusters before and after PCA

## Conclusion

This project demonstrates how clustering can be applied to cryptocurrency data and highlights the impact of dimensionality reduction on clustering results. PCA can simplify clustering without significantly losing meaningful information.
