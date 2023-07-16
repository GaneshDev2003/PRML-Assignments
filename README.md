# PRML-Assignments

This repository contains assignments/projects done in the course CS5691 Pattern Recognition and Machine Learning, done under the supervision of Prof. Arun Rajkumar at IITM. The assignments involved implementation of ML algorithms from scratch without using publicly available libraries (except numpy and pandas). More info can be found in the reports present in each folder.

## Assignment 1 - PCA and K-Means clustering

In this assignment, PCA was performed from scratch using numpy and pandas on the MNIST dataset. The principal components (i.e the eigen-vectors of the covariance matrix) were computed and shown as below. 

<img src = "https://github.com/GaneshDev2003/PRML-Assignments/assets/96174096/f8dd65bc-344b-48ab-8ef0-d6a3010eaa0d" width = "400"/>

Further they were reconstructed using the first few principal components, thus achieving dimensionality reduction for downstreaam tasks (d represents the number of principal components used). Thus a 28x28 image that required 784 features were reduced to around 60-70 features for downstream tasks.

<img src = "https://github.com/GaneshDev2003/PRML-Assignments/assets/96174096/95fc3861-e38c-4a40-968f-d709635f435e" width = "400"/>

Further, Kernel methods were used to caputure the non-linearity of the dataset. This was done using the RBF(Radial Basis Function) Kernel, and Polynomial Kernel.

K-means Clustering was performed on the crescent moon dataset and the following result was obtained.

<img src = "https://github.com/GaneshDev2003/PRML-Assignments/assets/96174096/9ee1efd2-ca5f-4a54-a565-f517aa1b635a" width = "400"/>

Further spectral clustering methods were employed to capture the non-linearity of the dataset, using RBF kernel and polynomial kernel.

## Assignment 2 - Regression

In this assignment, linear regression was done on a dataset with 100 features and 10,000 entries. It was done using the normal equations method , gradient descent method and stochastic gradient descent method. 

Ridge regression was also performed with 5-fold cross validation and found to have best results on the test data.

## Assignment 3 - Spam detection

Using this [Kaggle dataset](https://www.kaggle.com/datasets/venky73/spam-mails-dataset), a spam classifier was built.
First, the emails were preprocessed by removing stopwords, punctuations, etc. Then a count vectorizer was implemented using numpy.
Then, the classifier was built using : Naive Bayes and Logistic Regression. Out of these, logistic regression gave the highest accuracy.



