# Customer Segmentation

This repository contains the implementation of a customer segmentation project using the K-Means Clustering algorithm. The project involves clustering customers based on their annual income and spending score, with the optimal number of clusters determined using the Elbow Method.

## Table of Contents

- [Project Description](#project-description)
- [Business Use Case](#business-use-case)
- [Methodology](#methodology)
  - [K-Means Clustering](#k-means-clustering)
  - [Elbow Method](#elbow-method)
  - [Limitations](#limitations)

## Project Description

Customer segmentation is a crucial task for businesses to understand their customer base and tailor their marketing strategies accordingly. This project uses K-Means Clustering to segment customers based on their annual income and spending score, helping businesses identify distinct customer groups and target them more effectively.

## Business Use Case

Customer segmentation enables businesses to:
- Identify high-value customer segments and focus marketing efforts on them.
- Develop personalized marketing campaigns to improve customer engagement and retention.
- Optimize product offerings and services to meet the specific needs of different customer groups.
- Increase profitability by targeting the right customers with the right strategies.

## Methodology

### K-Means Clustering

K-Means Clustering is a popular unsupervised learning algorithm used to partition data into distinct clusters. In this project, we applied K-Means Clustering to group customers based on their annual income and spending score.

### Elbow Method

To determine the optimal number of clusters, we used the Elbow Method. This method calculates the within-cluster sum of squares (WCSS) and plots it against the number of clusters. The "elbow" point on the plot indicates the optimal number of clusters, where adding more clusters does not significantly reduce the WCSS.

### Limitations

While K-Means Clustering is effective for many scenarios, it has some limitations:
- The optimal number of clusters is determined manually, which can be subjective.
- K-Means is not suitable for datasets with overlapping centroids. Although DBSCAN can handle such cases, it was not used here as there was no problem of overlap in this dataset.
- There are warnings regarding the `n_init` parameter, but for better results, we have kept it auto.
