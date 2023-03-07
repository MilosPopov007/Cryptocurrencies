# Cryptocurrencies

Prominent investment bank, is interested in offering a new cryptocurrency investment portfolio for its customers.<br> The company, however, is lost in the vast universe of cryptocurrencies. So, they’ve asked me to create a report that includes what cryptocurrencies are on the trading market and how they could be grouped to create a classification system for this new investment.<br> The popularity of Bitcoin has caused a price jump.<br> That makes it unaffordable for many new investors.<br> There are many, many more cryptocurrencies available at more affordable prices.<br> Since there is no known output and the data is not ideal, this will be a perfect job for unsupervised machine learning. <br> <br>


![This is an image](https://github.com/MilosPopov007/Cryptocurrencies/blob/main/Resources/bitcoin-crypto-currency.jpg)



## Data Preprocessing:

I began the project by collecting cryptocurrency data from the CryptoCompare website using the API.<br>
We cleaned and preprocessed the data by dropping null values and non-cryptocurrency data.<br> Then, we standardized the data using the StandardScaler method from the scikit-learn library.<br> We used Principal Component Analysis (PCA) to reduce the dimensions of the data to three principal components to visualize the data in 3D.
