# Principal Component Analysis (PCA) and Customer Clustering

## Project Overview

This project focuses on conducting Principal Component Analysis (PCA) on customer data to extract key features and then performing unsupervised clustering to identify groups of similar customers. The steps involved in this analysis are outlined below.

## Steps

### 1. Load Data

The customer data is loaded from the "Customers.csv" CSV file into a Pandas dataframe named "data".

### 2. Select Variables for PCA

Variables for PCA are specified in a list named "features," including "Age," "Annual Income ($)," "Spending Score (1-100)," "Work Experience," and "Family Size."

### 3. Center and Standardize Data

Before applying PCA, the data is centered and standardized to ensure consistent scales for each variable.

### 4. Apply PCA

PCA is applied to the centered and standardized data using the PCA function from scikit-learn, calculating the principal components.

### 5. Calculate Explained Variances

The PCA function also calculates the proportion of variance explained by each principal component. These proportions are stored in a list named "explained_variances."

### 6. Visualize Explained Variances

A bar chart illustrating the proportion of variance explained by each principal component is plotted using the matplotlib library.

### 7. Select the Number of Components

The number of components to retain is chosen using the elbow rule, aiming for at least 80% of the total variance explained.

### 8. Reapply PCA

PCA is reapplied to the centered and standardized data using the selected number of components.

### 9. Add Principal Components to Original Dataframe

A new dataframe named "principalDf" is created to store the principal components extracted from PCA. This dataframe is then concatenated with the original "data" dataframe using the pandas concat function.

### Cercle de Corrélation

### 10. Perform Unsupervised Clustering

The KMeans clustering algorithm is used to perform unsupervised clustering on customers. We create 5 clusters using the hyperparameter n_clusters=5.

### 11. Add Cluster IDs to Final Dataframe

A new column named "Cluster" is added to the final dataframe containing cluster identifiers for each customer.

### 12. Display Variable Means by Cluster

Using the pandas groupby function, we calculate the means of each variable for each identified customer cluster. These means are then displayed for each variable and cluster.

## Getting Started

1. Clone the repository.
2. Set up a virtual environment and install dependencies.
3. Run the notebook 

## Contact

- [Mariem HSSINI](https://github.com/Mariemhssini))
- [Email](mailto:mariem.hassini@enicar.ucar.tn)

