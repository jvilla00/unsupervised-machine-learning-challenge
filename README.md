# Myopia Clusters

In this assignment, I used unsupervised machine learning by fitting data into a model and using clustering algorithms to place data into groups. Then, I created visualization that displayed these findings. 

## Background

The data science team of a medical research company is interested in finding better ways to predict myopia, or nearsightedness. The goal is to improve their classification model when training on a whole dataset. However, they believe that there might be distinct groups of patients that would be better to analyze separately. In hopes to achieve this I explored this possibility by using unsupervised learning.

I was provided with raw data, That I first needed to process to fit the machine learning models. Then I used several clustering algorithms to explore whether the patients can be placed into distinct groups. Then, I created visualizations that supported my findings.

## The Process

* Part 1: Prepare the Data

* Part 2: Apply Dimensionality Reduction 

* Part 3: Perform a Cluster Analysis with K-means

* Part 4: Make a Recommendation 

### Part 1: Prepare the Data

1. Read `myopia.csv` into a Pandas DataFrame.
2. Remove the "MYOPIC" column from the dataset.
3. Standardize the dataset so that columns that contain larger values did not influence the outcome more than columns with smaller values.

### Part 2: Apply Dimensionality Reduction

1. Perform dimensionality reduction with PCA. and not How did the number of the features changed.
2. Further reduce the dataset dimensions with t-SNE and visually inspected the results. I achieved this by, running t-SNE on the principal components, which is the output of the PCA transformation. 
3. Createed a scatter plot of the t-SNE output. and determined if there were distinct clusters?

### Part 3: Perform a Cluster Analysis with K-means

1. Created an elbow plot to identify the best number of clusters. 
2. Determined where the elbow of the plot was, and at which value of `k` it appeared.

### Part 4: Make a Recommendation

Based off the results from using the Dimensionality Reduction with PCA, there is variance in the first 3 features, when applying the t-SNE feature it is seprated into 5 clusters on the scatter plot. However once configuring the data into an elbow plot we can determine that the elbow bends at K=3. Meaning that any clusters after 3 are inconsequential. Inconclusion it is best to analyze the patients seperately as you can see in the charts provided.




