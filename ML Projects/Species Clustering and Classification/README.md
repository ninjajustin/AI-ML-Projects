# Species Clustering and Classification
In this assignment, I explored unsupervised clustering and outlier detection techniques to refine a synthetic dataset containing two features used to classify species. The objective was to clean noisy observations and build a reliable decision tree classifier based on refined clusters.

The process began by visualizing the dataset with a scatterplot to estimate the appropriate number of species (clusters), which was used as the parameter for clustering methods. I then identified the rough feature ranges that separated the species visually.

To detect and handle anomalies, I applied:

K-Means Clustering: Identified outliers by measuring distance from each cluster’s centroid.

DBSCAN Clustering: Used density-based clustering to detect noise points that didn’t belong to any dense region.

After detecting anomalies, I selected one clustering method to remove outlier data points and trained a Decision Tree Classifier on the cleaned dataset. The model was then visualized to interpret classification boundaries based on the two features.

Finally, I compared the classification performance before and after removing outliers to demonstrate how data cleaning improved the reliability and generalizability of the decision tree model.