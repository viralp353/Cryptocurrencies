# Cryptocurrencies

## Background:

In this challenge,Use unsupervised learning to analyze data on the cryptocurrencies traded on the market.



##  Objectives:


The goals for this challenge :

*  Prepare the data for dimensions reduction with PCA and clustering using K-means.


*  Reduce data dimensions using PCA algorithms from sklearn.


*  Predict clusters using cryptocurrencies data using the K-means algorithm form sklearn.


*  Create some plots and data tables to present your results:


## Challenge:



#### (1)Data Preprocessing:


Start by loading the data in a Pandas DataFrame named “crypto_df.” Continue with the following data preprocessing tasks:

*  Remove all cryptocurrencies that aren’t trading.


*  Remove all cryptocurrencies that don’t have an algorithm defined.


*  Remove the IsTrading column.


*  Remove all cryptocurrencies with at least one null value.


*  Remove all cryptocurrencies without coins mined.


*  Store the names of all cryptocurrencies on a DataFramed named coins_name, and use the crypto_df.index as the index for  this new DataFrame.


*  Remove the CoinName column.


*  Create dummies variables for all of the text features, and store the resulting data on a DataFrame named X.
Use the StandardScaler from sklearn (Links to an external site.) to standardize all of the data from the X DataFrame. Remember, this is important prior to using PCA and K-means algorithms.


#### (2)Reducing Data Dimensions Using PCA:

*  Once you have reduced the data dimensions, create a DataFrame named “pcs_df” that includes the following columns: PC 1, PC 2, and PC 3. Use the crypto_df.index as the index for this new DataFrame.


#### (3)Clustering Cryptocurrencies Using K-means:


*  Create an elbow curve to find the best value for K, and use the pcs_df DataFrame.


*  Once you define the best value for K, run the K-means algorithm to predict the K clusters for the cryptocurrencies’ data. Use the pcs_df to run the K-means algorithm.


*  Create a new DataFrame named “clustered_df,” that includes the following columns: Algorithm, ProofType, TotalCoinsMined, TotalCoinSupply, PC 1, PC 2, PC 3, CoinName, and Class


#### (4)Visualizing Results:

Complete the following tasks:

*  Create a 3D scatter plot using Plotly Express to plot the clusters using the clustered_df DataFrame. You should include the following parameters on the plot: hover_name="CoinName" and hover_data=["Algorithm"] to show this additional info on each data point.


*  Use hvplot.table to create a data table with all the current tradable cryptocurrencies. The table should have the following columns: CoinName, Algorithm, ProofType, TotalCoinSupply, TotalCoinsMined, and Class.


*  Create a scatter plot using hvplot.scatter to present the clustered data about cryptocurrencies having x="TotalCoinsMined" and y="TotalCoinSupply" to contrast the number of available coins versus the total number of mined coins. Use the hover_cols=["CoinName"] parameter to include the cryptocurrency name on each data point.




## Challenge_Summary:



##### (1)Data Preprocessing:


![Screenshot (124)](https://user-images.githubusercontent.com/65969608/95006920-29a54c00-05cf-11eb-86a5-9779576d8715.png)



##### (2)Reducing Data Dimensions Using PCA:

![Screenshot (125)](https://user-images.githubusercontent.com/65969608/95006927-4e99bf00-05cf-11eb-8b3d-6168011b81fd.png)

##### (3)Clustering Cryptocurrencies Using K-means:


![Screenshot (126)](https://user-images.githubusercontent.com/65969608/95006946-77ba4f80-05cf-11eb-8ee5-d9ec8bccabb0.png)


##### (4)Visualizing Results:

![Screenshot (127)](https://user-images.githubusercontent.com/65969608/95006958-9fa9b300-05cf-11eb-9a16-bbdc326b86fe.png)



![Screenshot (128)](https://user-images.githubusercontent.com/65969608/95006974-c667e980-05cf-11eb-8552-ad67a98fb5f0.png)





