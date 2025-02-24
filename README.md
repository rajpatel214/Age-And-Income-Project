# **Age and Income Clustering Analysis**  

## **Objective**  
The goal of this project is to analyze the relationship between **age and income** and segment individuals into distinct groups based on their income patterns. We apply **K-Means** and **DBSCAN** clustering techniques to categorize the data and compare their effectiveness in clustering.  

## **Dataset Overview**  
The dataset contains two key features:  
- **Age**: The age of individuals  
- **Income**: Their corresponding income  

This data is used to identify patterns in income distribution based on different age groups.  

## **Approach & Methodology**  

1. **Data Preprocessing**  
   - Checked for missing values and outliers.  
   - Scaled the data using **MinMaxScaler** to standardize the values for better model performance.  

2. **Clustering with K-Means**  
   - Applied the **Elbow Method** to determine the optimal number of clusters.  
   - Used **K-Means Clustering** with three clusters to group individuals based on income patterns.  
   - Plotted the clusters to visualize how income varies with age.  

3. **Clustering with DBSCAN**  
   - DBSCAN (Density-Based Spatial Clustering) was applied to find dense regions in the dataset.  
   - Experimented with different **epsilon (eps)** and **minimum samples** values to fine-tune the model.  
   - Compared clustering results with K-Means.  

## **Model Performance & Evaluation**  

- **K-Means Clustering Accuracy**  
  - **Silhouette Score**: **0.88**  
  - The model performed well in grouping similar individuals, but since K-Means is sensitive to outliers, results may not be stable for highly varying datasets.  

- **DBSCAN Clustering Accuracy**  
  - **Silhouette Score**: **0.77**  
  - Since DBSCAN is density-based, it handled noisy data better but was less effective due to variations in income distribution.  

## **Final Conclusion**  
- **K-Means** was more effective in identifying clear income-based clusters, given that the data was not highly dense.  
- **DBSCAN** struggled to segment the data effectively due to its sensitivity to the density of points.  
- K-Means is the preferred method for this dataset due to its ability to create well-defined clusters based on income and age patterns.  

This project highlights how **clustering techniques** can be used for market segmentation and customer profiling based on income distribution, making it useful for financial analysis, targeted marketing, and economic studies.
