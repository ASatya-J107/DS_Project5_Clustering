# Customer Segmentation Project

This project aims to perform customer segmentation using clustering techniques on the given dataset. Customer segmentation is a crucial step in marketing and business analytics as it helps identify distinct groups of customers with similar characteristics, behaviors, and needs. This information can be used to tailor marketing strategies and improve customer satisfaction.

## Dataset
The dataset used in this project can be found [dataset_link](https://raw.githubusercontent.com/ASatya-J107/DS_Project5_Clustering/main/segmentation_data.csv). It contains information about customers, including their sex, marital status, age, education, income, occupation, and settlement size.

## Data Preprocessing
- Imported necessary libraries, including pandas, numpy, matplotlib, seaborn, and warnings, and filtered out warnings.
- Loaded the dataset from a GitHub URL into a pandas DataFrame.
- Checked basic information about the dataset using `customer_info.info()`. The dataset has 2000 entries and 8 columns, all of which are numerical.

### Feature Types
- Numerical columns: 'ID', 'Age', 'Income'
- Categorical columns: 'Sex', 'Marital status', 'Education', 'Occupation', 'Settlement size'

## Data Distribution
- Performed data distribution analysis for numerical and categorical features.
- Visualized data distributions using histograms and count plots.

## Bivariate Analysis
- Conducted bivariate analysis to understand relationships between variables:
  - Pearson correlation coefficient between 'Age' and 'Income' is approximately 0.341, indicating a positive correlation.
  - Created scatter plots and regression plots to visualize the relationship between 'Age' and 'Income' for each category of categorical variables.

## Feature Transformation & Scaling
- Checked the normality of 'Income' and 'Age' using the normality test. Since both variables did not follow a normal distribution, applied data transformations:
  - Log transformation for 'Income'
  - Power transformation for 'Age'

### Feature Scaling
- Normalized the transformed features using MinMaxScaler.

## Clustering
- Performed customer segmentation using the K-Means clustering algorithm.
- Determined the optimal number of clusters (K) by evaluating the within-cluster sum of squares (inertia) for a range of K values.
- Chose K=6 or K=7 based on the elbow method and silhouette score analysis.

## Visualization
- Visualized the clusters in 3D space using PCA for dimensionality reduction.
- Created scatter plots to visualize the clusters based on the first three principal components.

## Results
- Segmented customers into 6 or 7 distinct clusters.
- Described each cluster's characteristics, including mean values for features.
- Visualized the distribution of features within each cluster.

## Conclusion
This customer segmentation analysis has successfully identified distinct customer clusters based on their demographic and socioeconomic characteristics. These clusters can be used to guide targeted marketing campaigns, personalize product recommendations, and enhance the overall customer experience. By tailoring strategies to specific customer segments, businesses can optimize their marketing efforts and improve customer satisfaction.

Furthermore, the insights gained from this analysis provide a foundation for data-driven decision-making. Businesses can use these clusters to refine their product offerings, optimize pricing strategies, and tailor communication to better meet the needs and preferences of each customer segment.

In conclusion, customer segmentation is a valuable tool for businesses looking to gain a competitive edge in today's data-driven marketplace. It allows for more effective and personalized customer engagement, ultimately leading to improved business outcomes.
