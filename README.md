# Online Retail Customer Segmentation

### Using RFM Analysis and Machine Learning Clustering

## Project Overview

This project performs **customer segmentation for an online retail business** using **RFM Analysis** and **Machine Learning clustering algorithms**.

Customer segmentation helps businesses understand different groups of customers based on their purchasing behavior, allowing companies to design **better marketing strategies, personalized promotions, and customer retention plans**.

The project uses the **Online Retail II dataset** and applies clustering techniques to group customers with similar behaviors.

---

# Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-Learn

---

# Machine Learning Algorithms Used

The following clustering algorithms are applied:

1. **K-Means Clustering**
2. **Hierarchical Clustering**
3. **DBSCAN Clustering**

Performance comparison is done using the **Silhouette Score**.

---

# RFM Analysis

RFM stands for:

* **Recency (R)** – Days since the customer's last purchase
* **Frequency (F)** – Number of purchases made by the customer
* **Monetary (M)** – Total amount spent by the customer

These three metrics help measure **customer value and engagement**.

---

# Project Workflow

## 1. Data Loading

The dataset is loaded using **Pandas** from an Excel file.

## 2. Data Cleaning

Data preprocessing includes:

* Removing rows with missing **Customer ID**
* Removing **cancelled orders**
* Creating a new feature **TotalPrice**

## 3. Feature Engineering

RFM features are calculated using:

* Recency
* Frequency
* Monetary Value

These features represent the purchasing behavior of each customer.

## 4. Data Transformation

To improve clustering performance:

* Log transformation is applied
* Outliers are removed using **IQR method**
* Data is standardized using **StandardScaler**

## 5. Clustering

Three clustering algorithms are used:

### K-Means Clustering

The **Elbow Method** determines the optimal number of clusters.

### Hierarchical Clustering

Groups customers based on hierarchical similarity.

### DBSCAN

Detects clusters based on density and identifies noise.

## 6. Model Evaluation

Cluster quality is evaluated using:

**Silhouette Score**

Higher values indicate better cluster separation.

## 7. Visualization

**PCA (Principal Component Analysis)** reduces data to **2 dimensions** for visualization.

A scatter plot shows customer segments visually.

## 8. Cluster Analysis

Each cluster's average **Recency, Frequency, and Monetary values** are analyzed to understand customer types.

Examples of segments:

* High-value loyal customers
* Frequent buyers
* Occasional shoppers
* At-risk customers

## 9. New Customer Prediction

The model allows predicting the **cluster for a new customer** by entering:

* Recency
* Frequency
* Monetary value

The trained model then assigns the customer to a segment.

---

# Output

The project provides:

* Customer clusters
* Silhouette scores
* PCA visualization
* Cluster summary analysis
* Prediction of new customer segment

---

# Business Benefits

Customer segmentation helps businesses:

* Identify **high-value customers**
* Improve **targeted marketing**
* Increase **customer retention**
* Optimize **sales strategies**

---

# Conclusion

This project demonstrates how **RFM analysis combined with machine learning clustering techniques** can effectively segment customers and provide valuable business insights.

The approach can be extended with **advanced machine learning models and real-time analytics** for large-scale retail systems.
