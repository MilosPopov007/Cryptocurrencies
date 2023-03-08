# [Cryptocurrencies](https://github.com/MilosPopov007/Cryptocurrencies/blob/main/crypto_clustering.ipynb)

Prominent investment bank, is interested in offering a new cryptocurrency investment portfolio for its customers.<br> The company, however, is lost in the vast universe of cryptocurrencies. So, they’ve asked me to create a report that includes what cryptocurrencies are on the trading market and how they could be grouped to create a classification system for this new investment.<br> The popularity of Bitcoin has caused a price jump.<br> That makes it unaffordable for many new investors.<br> There are many, many more cryptocurrencies available at more affordable prices.<br> Since there is no known output and the data is not ideal, this will be a perfect job for unsupervised machine learning. <br> <br>


![This is an image](https://github.com/MilosPopov007/Cryptocurrencies/blob/main/Resources/bitcoin-crypto-currency.jpg)



## Data Preprocessing:

I began the project by collecting cryptocurrency data from the CryptoCompare website using the API.<br>
We cleaned and preprocessed the data by dropping null values and non-cryptocurrency data.<br> Then, we standardized the data using the StandardScaler method from the scikit-learn library.<br> We used Principal Component Analysis (PCA) to reduce the dimensions of the data to three principal components to visualize the data in 3D.


## Cryptocurrency Clustering:

I used the K-means algorithm to cluster the cryptocurrencies into four different groups.<br>
We selected the optimal number of clusters by using the elbow curve.<br>
We created a new DataFrame with the scaled data, CoinName, and Class columns.<br><br>


![This is an image](https://github.com/MilosPopov007/Cryptocurrencies/blob/main/Resources/cluster_df.png)

![This is an image](https://github.com/MilosPopov007/Cryptocurrencies/blob/main/Resources/Elbow.png)

## Visualizing Cryptocurrencies:

We used various visualization techniques to analyze the cryptocurrency data, including a 3D scatter plot and 2D scatter plot.<br> We also created interactive visualizations using the hvplot library.<br><br>

![This is an image](https://github.com/MilosPopov007/Cryptocurrencies/blob/main/Resources/3D.png)<br><br>

The transformation of the tradable cryptocurrency data was done by using the MinMaxScaler() function.<br> This transformation was necessary to scale the TotalCoinSupply and TotalCoinsMined columns between the given range of zero and one, so that they can be used in the K-means clustering algorithm.

After the transformation, we created a new DataFrame with the scaled data, CoinName, and Class columns. We then used this DataFrame to create a scatter plot of the scaled TotalCoinsMined and TotalCoinSupply columns, which allowed us to visually inspect the distribution of the different cryptocurrency clusters.<br><br>


![This is an image](https://github.com/MilosPopov007/Cryptocurrencies/blob/main/Resources/scat_plot.png)


## Summary:

In conclusion, our analysis demonstrated the effectiveness of unsupervised machine learning in grouping and classifying cryptocurrency trading data. We were able to apply the K-means algorithm to identify meaningful patterns in the data and group the cryptocurrencies into four different clusters. This analysis was made possible through unsupervised machine learning, which enabled us to identify patterns in the data without prior knowledge of the outcome or any input-output pairs.

Our use of unsupervised machine learning in this analysis demonstrates the potential of this approach in identifying hidden patterns and grouping data in a wide range of applications. By using unsupervised machine learning, we can analyze data without the need for a labeled dataset, which is particularly useful in situations where data is unstructured or unknown. Furthermore, unsupervised machine learning can help to identify outliers, anomalies, and patterns in large datasets that are difficult to visualize or analyze manually.

Overall, we believe that unsupervised machine learning has significant potential in data analysis and can provide valuable insights into a range of applications. As more data becomes available, and more sophisticated machine learning techniques are developed, we anticipate that unsupervised machine learning will continue to play an essential role in data analysis and pattern identification.
