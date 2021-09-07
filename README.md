# Cryptocurrencies
Unsupervised Machine Learning with Cryptocurrencies

## Overview:
In this challenge we are given the task to use Scikit learn and Unsupervised Machine learning to cluster cryptocurrencies that are being traded on the market. There is no known output, so the idea is to let unsupervised ML do its job of clustering the crypto on the features we give it.

## Purpose:
The purpose of this challenge is to introduce unsupervised machine learning and the techniques of preparing and processing non ideal data to feed into our KMeans model. We will first preprocess the data, reduce the dimensions using the PCA statistics, cluster the crypto using the KMeans model, then visualize the results.             

## Resources
* Data Source: (crypto_data.csv)
* Software: 
\ Jupyter Notebook 6.3

## Analysis:
### Overview of Analysis:
Disclaimer, I don't believe I am competent enough in the statistical models being used to give an in-depth analysis of unsupervised ML. In summary, we are given a dataset that needs to be cleaned and processed. Once processed, we reduce the dimensions of the features using PCA. PCA uses linear algebra and eigenvectors/ eigenvalues to reduce the dimensions into 3 components. Each feature will have its own weight in the statistics. Once reduced, the K-means model is used to cluster the cryptocurrencies based on the 3 PCA. We use the KMeans to create an Elbow curve to determine how many clusters are used. After the clusters are created, we can create a clustered dataframe containing the cryptocurrencies and the clusters it has been assigned in. We can then graph the results in a 3D plot.

Before Scaling the data, the text features had to be converted to numerical values. 
![Get Dummies](https://github.com/lo7kyle/Cryptocurrencies/blob/main/Resources/texttonumbers.PNG) 
![Scaled Data](https://github.com/lo7kyle/Cryptocurrencies/blob/main/Resources/standardscalar.PNG) 

### Results:
From the results we are given 4 clusters and can see one outlier from the rest of the groups. We see that based on its PCA, it has the highest variance from the rest of the cryptocurrencies. 

Reduce the number of features using principal components
![Principal Component Analysis](https://github.com/lo7kyle/Cryptocurrencies/blob/main/Resources/3pca.PNG) 

To determine the cluster numbers, and Elbow curve was plotted. 
![Elbow Curve](https://github.com/lo7kyle/Cryptocurrencies/blob/main/Resources/Elbow_Curve.PNG) 
 
Once the PCA and KMeans model is completed, visualize the clustering. 
![3D Visualization](https://github.com/lo7kyle/Cryptocurrencies/blob/main/Resources/3d.PNG) 

To find out a more useful analysis regarding the features, we can plot a 2D graph of two specific features. In this case TotalCoinsMined vs TotalCoinSupply.
![2D Visualization](https://github.com/lo7kyle/Cryptocurrencies/blob/main/Resources/2d.PNG)
