# Fraud Detection Analysis Project

## 📌 Project Overview

This project focuses on analyzing financial transaction data to identify potentially fraudulent activities using unsupervised machine learning and anomaly detection techniques. The objective is not to create a production-level fraud detection system, but rather to gain hands-on experience with data exploration, preprocessing, clustering methods, and anomaly detection workflows.

**Project Goal:**
To analyze transaction patterns within banking data and uncover unusual behaviors that may indicate fraudulent activity while understanding the characteristics associated with high-risk transactions.

**Dataset Source:**
The dataset used for this project was obtained from Kaggle's Fraud Detection Dataset and is stored in the `data` directory as `bank.transaction.data.csv`.


## 🎯 Project Objectives

* Explore and understand transaction data using Exploratory Data Analysis (EDA) techniques
* Clean and preprocess the dataset through scaling and feature preparation
* Apply Principal Component Analysis (PCA) for dimensionality reduction and improved visualization
* Implement KMeans clustering and determine optimal clusters using evaluation metrics
* Identify suspicious transactions using Isolation Forest anomaly detection
* Create meaningful visualizations to communicate findings
* Generate insights related to transaction behavior and fraud patterns


## 🔧 Technologies and Methods Used

**Programming & Libraries**

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Plotly
* Scikit-learn
* SciPy

**Analytical Techniques**

* Data preprocessing and feature scaling
* Principal Component Analysis (PCA)
* KMeans clustering
* Isolation Forest anomaly detection

**Visualization Methods**

* Correlation heatmaps
* PCA scatter plots
* Cluster visualizations
* Distribution plots
* Geographic maps
* Trend and anomaly charts


## 📊 Important Findings

* Data preprocessing involved encoding categorical features, standardizing numerical variables, and removing irrelevant information to prepare the dataset for analysis.
* The optimal number of clusters was selected using silhouette scores and elbow curve analysis.
* PCA successfully reduced feature dimensions while maintaining important information and improving cluster visualization.
* Isolation Forest identified a small group of transactions as anomalous and potentially risky.
* Visual analysis highlighted clear differences between regular transactions and suspicious activity.


## 💡 Key Insights

### Cluster Analysis

**Cluster 0 – Middle-Aged Engineers**
Users in this cluster mainly consist of engineers with an average age of approximately 43 years. They maintain moderate account balances and perform medium-sized transactions with relatively shorter transaction durations.

**Cluster 1 – Young Students**
This group contains younger users with an average age near 23 years. They generally have lower account balances but show comparatively higher spending behavior relative to available funds.

**Cluster 2 – Retired Customers**
This cluster includes older individuals averaging around 60 years of age. These users possess higher balances and display stable, predictable transaction behavior.

**Cluster 3 – High-Balance Senior Customers**
This segment consists primarily of older users with the highest account balances and slightly higher login attempt counts, suggesting stronger security awareness or platform usability concerns.

Additional findings include:

* Most anomalous transactions were concentrated within Clusters 0 and 3.
* The number of suspicious transactions was significantly lower than normal transactions.
* Transactions classified as anomalies typically involved larger transaction amounts.
* Higher anomaly frequencies were observed on Fridays, around 6 PM, and during August, September, and November.
* Unusual transaction activity occurred more frequently during extremely short or very long transaction durations.
* Texas, Ohio, and Virginia showed the highest anomaly rates.
* Older users demonstrated a greater association with unusual activity patterns.
* Engineers and retired individuals showed higher levels of suspicious behavior compared to other occupations.
* Multiple login attempts strongly correlated with increased fraud risk.


## ⚠️ Project Limitations

* The dataset is synthetic and may not accurately reflect real-world transaction behavior.
* Essential business context and domain-specific rules are unavailable.
* Real-world fraud detection projects require continuous stakeholder feedback and iterative refinement.
* This project serves primarily as a learning exercise rather than a production-ready fraud solution.


## 📌 Future Improvements

* Explore alternative clustering approaches such as DBSCAN and Hierarchical Clustering.
* Implement supervised learning models if labeled fraud data becomes available.
* Include additional performance metrics such as Precision, Recall, and F1-score for better model evaluation.
