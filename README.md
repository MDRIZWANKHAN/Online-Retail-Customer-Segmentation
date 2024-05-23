# Online-Retail-Customer-Segmentation
![image](https://github.com/MDRIZWANKHAN/Online-Retail-Customer-Segmentation/assets/125923064/e91faf19-1ab7-4776-8bd7-0cd9cece108c)


Project Summary -
In this project, our task is to identify major customer segments on a transnational data set which contains all the transactions occurring between 01/12/2010 and 09/12/2011 for a UK-based and registered non-store online retail.The company mainly sells unique all-occasion gifts. Many customers of the company are wholesalers.
Problem Statement
A primary goal for any company and business is to understand their targeted customers. How their consumers operate and use their services. Every consumer may use a companies services differently. The problem we’re trying to solve is to define this delivery company’s consumers. To define certain behaviors and methods these consumers use the companies services for.
The optimal number of clusters for most of the models and data combinations is 2. The evaluation metrics considered in our project are silhouette score and the elbow method for K-means clustering.

To evaluate the positive business impact of the customer segmentation,the following evaluation metrics were considered:

Silhouette Score: The silhouette score measures the quality and compactness of the clusters. A higher silhouette score indicates well-separated clusters with minimal overlap. It provides a measure of how similar an object is to its own cluster compared to other clusters. Considering the silhouette score helps ensure that the identified clusters are distinct and meaningful, which can be beneficial for targeting specific customer segments with tailored marketing strategies.

Elbow Method: The elbow method is used to determine the optimal number of clusters based on the within-cluster sum of squares (WCSS) or the distortion. It involves plotting the WCSS as a function of the number of clusters and identifying the "elbow" point where the improvement in WCSS diminishes. The chosen number of clusters at the elbow point represents a trade-off between maximizing the separation of clusters and minimizing the complexity of the segmentation. This helps in finding a balance between granularity and practicality for business implementation.

The selection of these evaluation metrics indicates a focus on the quality of the clusters, their distinctiveness, and the ability to interpret and act upon the segmentation results. By considering these metrics, you aim to create customer segments that have clear boundaries and exhibit different behaviors or characteristics, which can lead to positive business impact through targeted marketing strategies, personalized customer experiences, and improved customer satisfaction.
Here i used K-means clustering.
K-means clustering is a popular and widely used algorithm for customer segmentation due to its simplicity, interpretability, and scalability.
Why i used,because-:

Scalability: K-means clustering is computationally efficient and can handle large datasets with a large number of customers. This is particularly important for online businesses that often have a vast amount of customer data.
Interpretability: K-means clustering produces easily interpretable results. The algorithm assigns each customer to a specific cluster based on their similarity in terms of feature values. The resulting clusters can be easily understood and analyzed to gain insights into customer behavior and characteristics.
Applicability to Online Data: K-means clustering can handle various types of features, including demographic information, purchase behavior, browsing patterns, or any other relevant data collected from online platforms. It can capture different aspects of customer behavior and group customers into distinct segments based on their similarities.
