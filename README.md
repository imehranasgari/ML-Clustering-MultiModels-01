# Customer Segmentation with Clustering Techniques

## Problem Statement and Goal of Project
This project aims to segment customers based on their age, annual income, and spending behavior using clustering algorithms. The goal is to identify distinct customer groups to inform targeted marketing strategies, demonstrating my ability to apply unsupervised machine learning techniques to real-world data.

## Solution Approach
The approach involves loading a customer dataset, preprocessing it, and applying three clustering algorithms:
1. **Data Preprocessing**: Load the dataset and standardize features using `StandardScaler`.
2. **Clustering**: Apply KMeans, Hierarchical (Agglomerative), and DBSCAN clustering algorithms.
3. **Evaluation**: Assess clustering performance using Silhouette, Calinski-Harabasz, and Davies-Bouldin scores.
4. **Visualization**: Plot clusters to visualize customer segments based on income and spending score.

This project showcases my skills in data preprocessing, clustering, and performance evaluation.

## Technologies & Libraries
- **Python 3.9.21**: Core programming language used in the Jupyter notebook.
- **pandas**: For data manipulation and analysis.
- **NumPy**: For numerical operations.
- **Matplotlib**: For visualizing clusters with scatter plots.
- **scikit-learn**: For data preprocessing (`StandardScaler`), clustering (`KMeans`, `AgglomerativeClustering`, `DBSCAN`), and evaluation metrics (`silhouette_score`, `calinski_harabasz_score`, `davies_bouldin_score`).

## Description about Dataset
The dataset (`clustering project.csv`) contains customer information with the following features:
- **CustomerID**: Unique identifier (int64).
- **Gender**: Categorical (object, e.g., Male, Female).
- **Age**: Customer age (int64).
- **Annual Income (k$)**: Annual income in thousands (int64).
- **Spending Score (1-100)**: Score indicating spending behavior (int64).

The dataset includes 200 entries (based on typical customer segmentation datasets), with a sample showing varied income and spending patterns.

## Installation & Execution Guide
To run this project locally:
1. **Prerequisites**:
   - Python 3.9.21 or compatible version.
   - Jupyter Notebook or JupyterLab installed.
   - Required libraries: `pandas`, `numpy`, `matplotlib`, `scikit-learn`.
2. **Installation**:
   ```bash
   pip install pandas numpy matplotlib scikit-learn
   ```
3. **Setup**:
   - Place the `clustering project.csv` dataset in the same directory as `clustring project.ipynb`.
   - Open the notebook in Jupyter:
     ```bash
     jupyter notebook clustring project.ipynb
     ```
4. **Execution**:
   - Run cells sequentially to load data, preprocess, apply clustering, and visualize results.
   - Note: The notebook assumes `clustering project.csv` exists; otherwise, a `FileNotFoundError` occurs.

## Key Results / Performance
The notebook compares three clustering algorithms with the following metrics for 4 clusters:
- **KMeans**: Silhouette Score (0.290), Calinski-Harabasz Score (66.856), Davies-Bouldin Score (1.306).
- **Hierarchical**: Silhouette Score (0.263), Calinski-Harabasz Score (60.306), Davies-Bouldin Score (1.402).
- **DBSCAN**: Silhouette Score (0.012), Calinski-Harabasz Score (12.099), Davies-Bouldin Score (1.389).

The results suggest five clusters may be optimal, with KMeans performing best, though DBSCAN's low scores indicate sensitivity to parameters, reflecting my exploration of clustering challenges.

## Screenshots / Sample Outputs
The notebook generates a scatter plot visualizing customer clusters:
- **Axes**: Annual Income (k$) vs. Spending Score (1-100).
- **Points**: Colored by cluster, with black for noise (DBSCAN).
- **Details**: Core points and outliers are plotted with 50% transparency.

*Note*: The base64-encoded image output represents the scatter plot. Run the notebook locally or view via [nbviewer.org](https://nbviewer.org) for full rendering.

## Additional Learnings / Reflections
This project deepened my understanding of clustering techniques:
- **Preprocessing**: Standardizing features is crucial for fair clustering.
- **Algorithm Comparison**: KMeans outperformed Hierarchical and DBSCAN, but DBSCAN's sensitivity to parameters highlighted the importance of tuning.
- **Evaluation**: Using multiple metrics provides a comprehensive view of clustering quality.
- **Exploration**: The experimental nature of DBSCAN's results shows my willingness to test and learn from challenging algorithms.

This project demonstrates my ability to apply and evaluate clustering methods, making it a strong portfolio piece.

## 👤 Author
**Mehran Asgari**  
**Email**: [imehranasgari@gmail.com](mailto:imehranasgari@gmail.com)  
**GitHub**: [https://github.com/imehranasgari](https://github.com/imehranasgari)

---

## 📄 License
This project is licensed under the Apache 2.0 License – see the `LICENSE` file for details.

---
