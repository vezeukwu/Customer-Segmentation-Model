## Customer Segmentation Model - Bethel Stores

![image](https://github.com/user-attachments/assets/7fdf92c6-b56f-477f-9b14-bbce58205a6a)


### Project Description:

Bethel Stores is a popular electronics retail chain that specializes in the sale of mobile phones, tablets, laptops, and other related accessories. The company was founded in 2020 and has since grown to become one of the largest retailers of mobile phones and related products in the country. Bethel Stores offers a wide range of mobile phones from top brands such as Samsung, Apple, Nokia, and Huawei, among others. The company is also known for its after sales support, including repairs and maintenance services, as well as trade in options for old devices. With its numerous outlets nationwide, Bethel Stores is a go to destination for many seeking to purchase mobile phones and related accessories.

### Problem Introduction and Objective
Bethel Stores wants to understand the spending behaviour of its customers in order to target them with personalized marketing campaigns. They have collected data on customer demographics (gender) and spending habits (annual income, spending score) and want to segment their customers based on their spending behavior.

The objective of this project is to build a customer segmentation model to help the retail store in developing targeted marketing strategies.

### Feature Description
Bethel Stores collected data on 200 customers containing:
• CustomerID

• Gender

• Age

• Annual_Income (k$)

• Spending_Score

### Data Preparation (EDA)
•	Loading the Data

•	Data Cleaning and Handling Missing Data

•	Univariate and Bivariate Analysis

•	Machine Learning using Clustering-(KMeans)

•	Summarizing and Visualization

### Analysis Summary
In this analysis, I aimed to build a machine learning model that can successfully segment customers according to their income level and spending habits based on the given features. My workflow included data preparation, Exploratory data analysis, Model training exploring the Kmeans – clustering – an unsupervised machine learning model to segment customers based on their Annual Income (k$) and Spending Score.

Below is a summary of each step:

Data Cleaning and Transformation:  I checked for missing values and data inconsistencies and outliers in the dataset, examined the relationships between the features and visualizing them using the univariate and bivariate analysis to maintain model integrity and ensure logical consistency across the dataset.

Model Selection and Optimization:
K-means clustering algorithm was used to determine the optimal number of clusters using the Elbow method. This method involves plotting the Within Cluster Sum of Squares (WCSS) against the number of clusters (K) and Selecting the value of K where the rate of decrease in WCSS slows down significantly. In the Elbow graph, we can observe that after K=5, there is no significant decrease in WCSS, indicating that 5 is the optimal number of clusters in this case.

Model Training:
The K-Means model was fitted with 5 clusters using the k-means++ initialization to optimize the centroid placement and ensure convergence. Cluster labels were added to the dataset for further analysis.

Visualization:
A scatter plot was created to visualize the clustering results, plotting Annual Income (k$) on the x-axis and Spending Score on the y-axis. Clusters were color-coded for clear differentiation.

Evaluation:
The silhouette score, a metric for evaluating the quality of clustering, was calculated to be approximately 0.44, indicating moderately well-defined clusters.

### Conclusion and Recommendations
The customer segmentation project successfully categorized customers into five distinct groups based on their Annual Income and Spending Score. These insights provide valuable opportunities for targeted marketing and tailored services:

High-income, high-spending customers to be prioritized for premium offerings and loyalty programs.

Low-income, low-spending customers may require affordable options or basic products.

Wealthy but cautious spenders to be engaged with personalized recommendations or savings-driven incentives.

Although the clustering revealed meaningful patterns, the moderate silhouette score suggests the need for further exploration.
