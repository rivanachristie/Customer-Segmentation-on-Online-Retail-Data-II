# Customer-Segmentation-on-Online-Retail-Data-II

Project by: Rivana Christie and Pratik Dahibhate

As part of this project, we are using dimensionality reduction and clustering to segment the users from an online retail dataset. We use principal component analysis (PCA) for dimensionality reduction. Then we apply the following clustering techniques on the reduced dataset:

1. K-Means Clustering
2. K-Mean Mini Batch Clustering
3. Gaussian Mixture Model

Furthermore, we perform RFM segmentation on the dataset to segment the users based on their spending habits using the following clustering algorithms:

1. K-Means Clustering
2. Spectral Clustering
3. Gaussian Mixture Model

## About the dataset
This Online Retail II data set contains all the transactions occurring for a UK-based and registered, non-store online retail between 01/12/2009 and 09/12/2011.The company mainly sells unique all-occasion gift-ware. Many customers of the company are wholesalers.

Link to dataset: https://archive.ics.uci.edu/ml/datasets/Online+Retail+II

## Data Cleaning:
As part of data cleaning, the following steps are performed:

1. Removing NA or null values
2. Converting 'Description' column to lower case
3. Converting 'InvoiceDate' to a datetime column
4. Removing cancelled orders from the dataset
5. Creating a 'TotalPrice' column

## Exploratory Data Analysis (EDA)
1. Top 10 countries with highest spending:
![image](https://github.com/rivanachristie/Customer-Segmentation-on-Online-Retail-Data-II/assets/98617715/c45940a7-d25c-4c4a-bf11-450e743feccc)

2. Purchase trend over time:
![image](https://github.com/rivanachristie/Customer-Segmentation-on-Online-Retail-Data-II/assets/98617715/0c2fa99d-3cbd-4906-af8e-4be2235c9222)

3. Top 10 most purchased items:
![image](https://github.com/rivanachristie/Customer-Segmentation-on-Online-Retail-Data-II/assets/98617715/cc661250-7c09-4940-b3f8-8642a185d077)

## Data Preprocessing and Dimensionality Reduction using Principal Component Analysis (PCA):
As part of data preprocessing:

1. Firstly, we use the label encoder to encode the categorical columns into numerical values
2. Then, we use StandardScaler() to scale the values and thus reduce outliers
3. Finally, we use PCA to reduce the number of dimensions to 3

![image](https://github.com/rivanachristie/Customer-Segmentation-on-Online-Retail-Data-II/assets/98617715/ce43d747-424f-4398-8e6d-6ab93b6bf8ad)

## Data Modeling:
Firstly, we get the optimal number of clusters using the K-Means Elbow Method. Then, we use the clustering techniques to get the clusters of the users.

![image](https://github.com/rivanachristie/Customer-Segmentation-on-Online-Retail-Data-II/assets/98617715/2c2c990c-5cf8-4da0-b7d8-61baf387eb77)

1. K-Means Clustering:
![image](https://github.com/rivanachristie/Customer-Segmentation-on-Online-Retail-Data-II/assets/98617715/7e5acce3-4683-4f2e-a1de-966e38e73bd8)

2. Guassian Mixture Model (GMM):
![image](https://github.com/rivanachristie/Customer-Segmentation-on-Online-Retail-Data-II/assets/98617715/2ebd284e-aace-4236-a1a9-7ee40306571a)

3. K-Means Mini Batch Clustering:
![image](https://github.com/rivanachristie/Customer-Segmentation-on-Online-Retail-Data-II/assets/98617715/afd30f17-5067-4462-ac67-2dc1bf25b4de)

## Model Evaluation:

1. Model training with PCA:

| Model | Silhouette Score |
| K-Means Clustering | 0.3887 |
| Guassian Mixture Model | 0.389 |
| K-Means Mini Batch Clustering | 0.3568 |

2. Clustering using RFM Segmentation:

| Model | Silhouette Score |
| K-Means Clustering | 0.3887 |
| Guassian Mixture Model | 0.389 |
| K-Means Mini Batch Clustering | 0.3568 |







