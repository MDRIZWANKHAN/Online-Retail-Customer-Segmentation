# Online-Retail-Customer-Segmentation
![image](https://github.com/MDRIZWANKHAN/Online-Retail-Customer-Segmentation/assets/125923064/e91faf19-1ab7-4776-8bd7-0cd9cece108c)


### ***Project Summary*** 
In this project, our task is to identify major customer segments on a transnational data set which contains all the transactions occurring between 01/12/2010 and 09/12/2011 for a UK-based and registered non-store online retail.The company mainly sells unique all-occasion gifts. Many customers of the company are wholesalers.

### ***Problem Statement***
A primary goal for any company and business is to understand their targeted customers. How their consumers operate and use their services. Every consumer may use a companies services differently. The problem we’re trying to solve is to define this delivery company’s consumers. To define certain behaviors and methods these consumers use the companies services for.

### ***Approaches***
we will break this endeavor into different parts-:
### ***EDA***
- In this i have created different charts like Bar, Kde, Histogram, Box, Heatmap and Pair Plot for getting insights from the data and based on that we can do some feature Engineering.
- I also performed Hypothesis Testing based on our findings.

### ***Creating RFM Model***
Before applying any clustering algorithms it is always necessary to determine various quantitative factors on which the algorithm will perform segmentation. Examples of these would be features such as amount spend, activeness of the customer, their last visit, etc.

RFM model which stands for Recency, Frequency, and Monetary is one of such steps in which we determine the recency - days to last visit, frequency - how actively the customer repurchases and monetary - total expenditure of the customer, for each customer. There are other steps too in which we divide each of these features accordingly and calculate a score for each customer. However, this approach doesnot require machine learning algorithms as segmentation can be done manually. Therefore we will skip the second step and directly use the rfm features and feed it to clustering algorithms.
To evaluate the positive business impact of the customer segmentation,the following evaluation metrics were considered:
          - Recency = Latest Date - Last Inovice Data,
          - Frequency = count of invoice no. of transaction(s)
          - Monetary = Sum of Total Amount for each customer

### ***Segmentation with K-means clustering:***
   ***Applied Silhouette Score Method on Recency and Monetary*** and ***Applied Elbow Method on Recency and Monetary*** we see that ,Customers are well separate when we cluster them by Recency and Monetary.
   ***Applied DBSCAN Algorithm on Recency and Monetary*** we see that ,Customers are well separate when we cluster them by Frequency and Monetary.
   ***Applied Hierarchical Clustering*** i get No. of Cluster = 2.
   
- Here i used K-means clustering.
- K-means clustering is a popular and widely used algorithm for customer segmentation due to its simplicity, interpretability, and scalability.

### ***Conclusion***
The analysis we went through various steps to perform customer segmentation. We started with data wrangling in which we tried to handle null values, duplicates and performed feature modifications. Next, we did some exploratory data analysis and tried to draw observations from the features we had in the dataset.

Next, we formulated some quantitative factors such as recency, frequency and monetary known as rfm model for each of the customers. We implemented KMeans clustering algorithm on these features. We also performed silhouette and elbow method analysis to determine the optimal no. of clusters which was 2. We saw customers having high recency and low frequency and monetary values were part of one cluster and customers having low recency and high frequency, monetary values were part of another cluster.

However, there can be more modifications on this analysis. One may choose to cluster into more no. depending on company objectives and preferences. The labelled feature after clustering can be fed into classification supervised machine learning algorithms that could predict the classes for new set of observations.
