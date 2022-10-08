# Cryptocurrencies
## Purpose:
### The purpose of this analysis was to use data from CryptoCompare to provide a report that includes, what cryptocurrencies are on the trading market and how they could be grouped to create a classification system, for this new investment and visualization of currently traded cryptocurrencies that can be grouped together to create a new classification system. This report would be used to help Accountability Accounting, offers a new investment portfolio in the exciting world of cryptocurrency to its customers. The data Martha will be working with is not ideal, so it will need to be processed to fit the machine learning models. Since there is no known output, we decided to use unsupervised learning, and to group the cryptocurrencies, we are using a clustering algorithm. We’ll use data visualizations to share findings, for that we are Preprocessing data (Selection, Transformation, Scaling) for unsupervised learning and the process of helping to prepare data for Machine Learning Algorithms, Cluster data using the K-means algorithm.  Since the data does not have any known outcome, we needed to preprocess it to fit an unsupervised Machine Learning model that will enable us to run a clustering algorithm, that will allow us to group the cryptocurrencies.
## Results:
### The original dataset contained 1,252 entries, however only 1,144 cryptocurrencies were currently trading. The data was further munged to remove null values and only leave cryptocurrencies that had a total number of mined coins greater than 0. The final results identified 532 tradable cryptocurrencies.
![Crypto_DF Image](https://github.com/Rubina-Shrivastava/Cryptocurrencies/blob/main/Images/crypto_df.png)

### Tradable Cryptocurrencies Table: Most of the cryptocurrencies are part of classes #0 and #3
![Cluster_DF Image](https://github.com/Rubina-Shrivastava/Cryptocurrencies/blob/main/Images/clustered_df.png)

### We are creating an elbow curve using hvPlot to find the best value for K from the pcs_df DataFrame
![Hvplot Image](https://github.com/Rubina-Shrivastava/Cryptocurrencies/blob/main/Images/hvplo.table.png)

### The PCA algorithm reduces the dimensions of the X DataFrame down to three principal components, pcs_df DataFrame is created and has the following three columns, PC 1, PC 2, and PC 3, and has the index from the crypto_df DataFrame
![Pcf_DF Image](https://github.com/Rubina-Shrivastava/Cryptocurrencies/blob/main/Images/pcs_df.png)

### Unsupervised machine learning was used to identify clusters of the cryptocurrencies the K-Means method iterating from 1 to 10 . The best K value is 4 so we would conclude on 4 clusters in our output. The K-means algorithm is used to cluster the cryptocurrencies using the PCA data.
![Bokenplot(1) Image](https://github.com/Rubina-Shrivastava/Cryptocurrencies/blob/main/Images/bokeh_plot%20(1).png)

## 2D-Scatter plot with TotalCoinMined vs TotalCoinSupply
### Plotting the scatter plot from two cryptocurrency features Using the PCA algorithm is the best method for better visualizations
![Bokenplot Image](https://github.com/Rubina-Shrivastava/Cryptocurrencies/blob/main/Images/bokeh_plot.png) 

## 3D-Scatter plot with clusters
### The PCA algorithm is used to reduce the cryptocurrencies dimensions to three principal components. in this 3-D scatter plot
![Newplot Image](https://github.com/Rubina-Shrivastava/Cryptocurrencies/blob/main/Images/newplot.png)

## Summary:
###   We did identify the classification 0f 531 cryptocurrencies based on similarities of their features The output is unknown, the best method would be unsupervised learning and clustering algorithms to group the currencies This classification report could be used by an investment bank to propose a new cryptocurrency investment portfolio to its clients.
