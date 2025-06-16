# 🛍️ Mall Customer Segmentation using KMeans Clustering

This project performs **unsupervised clustering analysis** on mall customer data to segment customers based on their **Annual Income** and **Spending Score**. The goal is to identify distinct groups of customers that can help with targeted marketing strategies and business decisions.

## 📁 Dataset

- **File:** `Mall_Customers.csv`
- **Features used for clustering:**
  - Annual Income (k$)
  - Spending Score (1-100)

> **Note:** Columns such as `CustomerID`, `Gender`, and `Age` are dropped to focus purely on clustering behavior.

## 🔄 Project Workflow

### 🔹 1. Data Collection
- Load the dataset using `pandas`.
- Preview the dataset using `.head()` and check for data types using `.info()`.

### 🔹 2. Data Preprocessing
- Drop irrelevant columns (`CustomerID`, `Gender`, `Age`).
- Check and confirm absence of missing values.
- Standardize the data using `StandardScaler` to bring all features to the same scale.

### 🔹 3. Determine Optimal Number of Clusters
- **Elbow Method**: 
  - Calculate Within-Cluster Sum of Squares (WCSS) for `k = 1 to 10`.
  - Plot the elbow curve to find the "elbow point".
- **Silhouette Score**:
  - Calculate silhouette score for `k = 2 to 10` to measure how well clusters are formed.

### 🔹 4. Build Final KMeans Model
- Choose optimal number of clusters (e.g., `k = 5`).
- Train the KMeans model with the scaled data.
- Predict cluster labels for each data point.

### 🔹 5. Cluster Visualization
- Plot the clusters in a 2D scatter plot using `matplotlib`.
- Each cluster is color-coded automatically.
- Cluster centroids are marked with a black "X".

---

## 📊 Evaluation Techniques

### ✅ Elbow Method
Used to identify the optimal number of clusters based on WCSS.

### ✅ Silhouette Score
Evaluates how well each point lies within its cluster vs. others.

---

## 📈 Final Output

- Identified **5 distinct customer segments**.
- Visualized clusters based on spending behavior and income.
- Clustering can assist with targeted marketing strategies, loyalty programs, and personalized recommendations.

## 📬 Contact

For any queries or suggestions, feel free to reach out:

- 📧 Email: [abineshbalasubramaniyam@example.com](mailto:abineshbalasubramaniyam@example.com)
- 💼 LinkedIn: [linkedin.com/in/abinesh-b-1b14a1290/](https://www.linkedin.com/in/abinesh-b-1b14a1290/)
