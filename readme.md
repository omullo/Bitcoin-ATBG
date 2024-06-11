
# README for BitcoinATBG Visualization Notebook

## Overview

This Jupyter Notebook is designed to visualize a bipartite graph representing Bitcoin transactions and addresses using the `ipycytoscape` library. The dataset contains transactions from January 3, 2009, to June 7, 2018. It maps addresses and transactions from the raw Bitcoin blockchain to numerical vertex IDs, creating a comprehensive bipartite graph.

## Dataset Information

**Name**: BitcoinATBG

**Description**: The dataset is a Bitcoin addresstransaction bipartite graph, spanning over 9.5 years of transactions. It includes mappings from Bitcoin transactions and addresses to numerical vertex IDs. This bipartite graph consists of:
 **Transactions**: 321,043,952 (321 million)
 **Addresses**: 399,344,696 (399 million)
 **Total Vertices**: 720,388,650 (720 million)
 **Total Edges**: 1,692,308,191 (1.6 billion)

**Formats**:
1. **Matrix Market Exchange Format (.mtx)**: ASCII file format.
2. **Compressed Sparse Row (CSR)**: Binary format.
3. **Sample Graphs**: Included in both Matrix Market and CSR formats for demonstration.

## Notebook Instructions

### Purpose

The notebook demonstrates the following:
1. Fetching and parsing JSON data from an API.
2. Processing and extracting relevant parts of the dataset.
3. Creating node and edge data structures.
4. Visualizing the bipartite graph using `ipycytoscape`.
5. Performing key statistical analyses.
6. Applying Machine Learning (ML) and Deep Learning (DL) techniques for advanced data analysis.
### Setup and Running the Notebook

1. **Install Jupyter Notebook**:
   Ensure you have Jupyter Notebook installed. If not, install it using pip:
   \`\`\`sh
   pip install notebook
   \`\`\`

2. **Install Required Packages**:
   Install the necessary Python packages:
   \`\`\`sh
   pip install requests pandas ipycytoscape
   \`\`\`

3. **Launch Jupyter Notebook**:
   Start Jupyter Notebook from the command line:
   \`\`\`sh
   jupyter notebook
   \`\`\`

4. **Open and Run the Notebook**:
    Open the provided notebook file in Jupyter Notebook.
    Execute each cell sequentially to fetch data, process it, and visualize the graph.
    The final cell will display the bipartite graph using `ipycytoscape`.
# Getting the Data

If you want to download the dataset to your local machine, you can retrieve it from the Oracle Open Data repository using the following command:
 \`\`\`sh
   curl https://api.opendata.ocs.oraclecloud.com/data/landsat-4-5-tm/ -o bitcoin-atbg-dataset.zip
   \`\`\`

# Statistical Analyses

The notebook includes several key statistical analyses:

## Descriptive Statistics
 **Summary Statistics**: Provides mean, median, standard deviation, minimum, and maximum values.
 **Advanced Descriptive Statistics**: Includes skewness and kurtosis for transaction amounts.

## Correlation Analysis
 **Correlation Matrix**: Displays the linear relationships between different numerical features using a heatmap.

## Hypothesis Testing
 **TTest**: Compares transaction amounts between different addresses.
 **ANOVA**: Compares means across multiple groups.

## Regression Analysis
 **Linear Regression**: Models the relationship between transaction amounts and features such as address ID and date.
 **Neural Network Regression**: Uses a neural network to predict transaction amounts.
 **Residual Analysis**: Plots residuals to check the assumptions of the regression model.

## Time Series Analysis
 **Decomposition**: Decomposes the time series data to identify trends, seasonality, and residual components.
 **Autocorrelation Analysis**: Uses the Autocorrelation Function (ACF) to analyze the correlation of the time series with its own past values.
 **LSTM for Time Series Forecasting**: Uses LSTM networks to forecast future transaction amounts.

## Clustering
 **KMeans Clustering**: Groups transactions into clusters based on amount and address ID.

# Machine Learning and Deep Learning Techniques

## Machine Learning
 **Linear Regression**: Predict transaction amounts using a linear model.
 **Random Forest Classifier**: Classify transactions based on features.

## Deep Learning
 **Neural Network**: Predict transaction amounts using a neural network.
 **LSTM for Time Series Forecasting**: Forecast future transaction amounts using LSTM for time series data.

# Visualizations

Several captivating visualizations are included to help understand the data better:
 **Distribution of Transaction Amounts**: Using histograms and violin plots.
 **Transaction Amounts Over Time**: Using line plots.
 **Box Plot of Transaction Amounts by Address**: Comparing transaction amounts across different addresses.
 **Heatmap of Transaction Counts by Date and Address**: Showing the frequency of transactions over time for different addresses.
 **PCA Scatter Plot**: Showing principal components and clustering results.
 **Neural Network Predictions**: Plotting actual vs predicted transaction amounts.
 **LSTM Predictions**: Plotting actual vs predicted transaction amounts for time series data.

# Conclusion

This notebook provides a comprehensive guide to processing, visualizing, and analyzing a subset of the BitcoinATBG dataset. It showcases the use of various Python libraries to handle, visualize, and perform advanced analyses on large bipartite graphs within a Jupyter Notebook environment. By following the instructions and running the provided code, you can gain deeper insights into the data and understand the relationships and patterns within the dataset.


