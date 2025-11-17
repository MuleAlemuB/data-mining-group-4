Title :Mall Customer Segmentation using K means clustering

Project Overview
This project performs customer segmentation on a mall's customer dataset to identify distinct groups based on their spending behavior and annual income. The analysis helps in understanding customer profiles, which can guide marketing strategies and business decisions.

The dataset used is `Mall_Customers.csv`, which contains attributes such as CustomerID, Gender, Age, Annual Income (k$), and Spending Score (1-100).

Objectives
- Segment customers into meaningful groups using K-Means Clustering.
- Visualize clusters and understand patterns in customer behavior.
- Identify key insights such as high-value customers or low-spending groups.
- Save the processed data and trained model for further analysis or deployment.

 Key Steps
1. Data Loading – Import the dataset into a Pandas DataFrame.
2. Exploratory Data Analysis (EDA) – Visualize distributions, correlations, and relationships.
3. Data Preprocessing – Handle missing values, encode categorical variables, and prepare features.
4. Feature Selection – Use relevant features (`Annual Income`, `Spending Score`) for clustering.
5. Modeling – Apply K-Means Clustering to segment customers.
6. Cluster Evaluation – Analyze Inertia and Silhouette Score to determine optimal clusters.
7. Visualization – Plot clusters and centroids for clear interpretation.
8. Export Results – Save clustered data as `Mall_Customers_Segmented.csv` and trained model as `kmeans_mall_model.pkl`.

 Key Results
- Total Clusters Formed: 5  
- Inertia (Sum of squared distances): 169.89  
- Silhouette Score: 0.3883
-  
INTERPRETATION OF CLUSTERS
Cluster 0 → High Income – High Spending (Premium Customers)
Cluster 1 → Low Income – High Spending (Impulsive Buyers)
Cluster 2 → Medium Income – Medium Spending (Average Customers)
Cluster 3 → Low Income – Low Spending (Low-Value Customers)
Cluster 4 → High Income – Low Spending (Careful / Budget-conscious Customers)

Cluster Visualization
![Cluster Visualization](https://github.com/MuleAlemuB/data-mining-group-4/blob/main/images/download%20(5).png?raw=true)
![Cluster Visualization](https://github.com/MuleAlemuB/data-mining-group-4/blob/main/images/download%20(6).png?raw=true)


### Cluster Centroids
| Cluster | Annual Income (k$) | Spending Score (1-100) |
|---------|------------------|------------------------|
| 1       | 25.9             | 79.3                   |
| 2       | 26.0             | 20.5                   |
| 3       | 65.6             | 82.0                   |
| 4       | 69.0             | 20.9                   |
| 5       | 88.5             | 50.6                   |

Files
- `Mall_Customers.csv` – Original dataset
- `data-mining-final.ipynb` – Jupyter Notebook with all analysis and visualization
- `Mall_Customers_Segmented.csv` – Dataset with cluster labels
- `kmeans_mall_model.pkl` – Saved K-Means model

Tools & Libraries
- Python 3
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn (KMeans, preprocessing)
- Google Colab

Usage
1. Clone this repository.
2. Open `data-mining-final.ipynb` in Jupyter or Google Colab.
3. Run all cells sequentially to reproduce the results.
4. Visualize clusters and check the exported CSV for segmented data.

Author
Group 4 students 
Debre Tabor University  
4th Year Computer Science Students
