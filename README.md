# Crypto Clustering

## Objective
The objective of this project is to use machine learning to group cryptocurrencies into like clusters using both original, normalized data, and a PCA approach. The different approaches are then compared to determine the impact of using PCA vs. original, normalized data.

## Methods Used

This project uses the Scikit-Learn, or Sklearn, library in Python. The StandardScaler function is used first to normalize the data in the csv file. Then, the KMeans is used in a loop through the data and the inertia for our K values are stored in a list. These K values and inertia values can then be graphed to determine our ideal value of K for our machine learning model. For this project, the ideal value of K is 4. We now know the ideal number of clusters and can plug that number into our model prediction and graph our clustered data in a scatter plot.

The next step of this project is to rerun our clustering analysis, this time using a PCA approach. We utilize a PCA and set the number of components equal to 3. In other words, we are reducing all our data down to 3 columns. We run the explained_variance_ratio_ function to see our total explained variance of the three components, 0.895. This is a relatively high explained variance ratio and tells us we can run our PCA model with 3 components without sacrificing much accuracy in our analysis. 

The last step of this project is to rerun our machine learning model with our new PCA values. Our new elbow graph shows that we will still use 4 clusters in our model and display them in a new scatter plot. We then overlay our original and PCA graphs to compare the different outcomes.

## Outcome

The outcome of this project shows that using a PCA approach in this case did not sacrifice any noticable amount of accuracy in our final outcome. The crypto clusters appear to be clustered the same between approaches, and the same number of clusters were used.
