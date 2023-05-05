#  CryptoClustering
##  Module 19 HW Assignment


In this challenge, you’ll use your knowledge of Python and unsupervised learning to predict if cryptocurrencies are affected by 24-hour or 7-day price changes.

## Methods:

* Load and preprocess the data
* Normalize the data using StandardScaler
* Find the best value for k using the elbow method
* Cluster the data with K-Means using the original data market_data_df2
* Run PCA to reduce the dimensions  to three principal components
* Re-evaluate the best value for k using the elbow method
* Cluster the PCA driven data
* Visualize and compare composite plots of both the elbow plots and K-Means cluster plots.
* Determine the impact the reduction of feautures has on the data.

## Results:

#### __Original crypto currency data looking at the price change percentages over the course of different time durations__ 
![Screenshot 2023-05-04 at 10 01 44 PM](https://user-images.githubusercontent.com/119906575/236380790-d97184b5-e4c7-4b01-8d4f-9145a673965c.png)

![bokeh_plot](https://user-images.githubusercontent.com/119906575/236381701-540ebcff-1a49-441f-aba9-c145828c8274.png)
#### K-Means Cluster for Crypto Currency Data
![bokeh_plot-2](https://user-images.githubusercontent.com/119906575/236381816-54519d0f-38f9-47cb-947b-004fe0d6f18e.png)

![bokeh_plot-3](https://user-images.githubusercontent.com/119906575/236381875-96d3b11d-9d87-4de8-8c30-1d5cd472dbe2.png)
#### K-Means Cluster for PCA
![bokeh_plot-4](https://user-images.githubusercontent.com/119906575/236381915-f3dec832-7300-4e10-9905-ffa28208c862.png)

## Question: 

* After visually analyzing the cluster analysis results, what is the impact of using fewer features to cluster the data using K-Means?

## Answer: 

* The impact of utilizing a principal component analysis is that by reducing the dimensions tested, the algorithm makes the data simplier to explore. Our first K-Means clusters plotted are not highly segregated. The inflection point on both elbow plots are at the same point, determining 4 clusters is our optimal cluster count. The PCA plot reduces the dimensions of our data removing outliers from our plot, making it clearer to distinguish the data.

## Dependencies

* Pandas
* Hvplot.pandas
* Sklearn
* KMeans from sklearn.cluster
* PCA from sklearn.decomposition
* StandardScaler from sklearn..preprocessing
