# Cryptocurrencies

## Overview
This analysis is about grouping Cryptocurrencies using unsupervised learning. The dataset was retrieved from CryptoCompare and contained coins name, the algorithm they use, whether trading on the market or not, proof type, total coins minded, and total coin supply. 

## Procedure
The first coins are filtered to ones with a working algorithm and traded in the market for preprocessing. Then all rows containing null values are eliminated. After that, text features are converted to variables using "get_dummies()." Furthermore, it standardized using "StandardScaler()."

In the next step, features are reduced to three principal components using PCA. K-Means clustering is used for grouping cryptocurrencies, So before that Elbow curve is drawn to find the best value for K.

Behind classification, results are visualized using "Plotly" and "Hvplot."

## Results
- The Elbow curve revealed the optimum number of clusters to classify our coins is K=4.
![This is an image](/ElbowCurve.jpg)

- Five hundred thirty-two coins are classified into four classes.
![This is an image](/Table.jpg)

- Most of coins are classified in group 0 or 1.
![This is an image](/3DScatterPlot.jpg)
