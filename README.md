# Unsupervised Learning: Clustering Project

This project explores multiple clustering algorithms in unsupervised learning and demonstrates how cluster labels can be used as new features to improve supervised models. The work includes implementing clustering methods, evaluating them, tuning hyperparameters, and integrating cluster-based features into a Lasso Regression model.

---

## Project Objectives

- Understand and implement major clustering algorithms.
- Tune and evaluate clustering models using Distortion and Silhouette Score.
- Use cluster assignments as new features in a supervised learning model.
- Compare clustering approaches by complexity, speed, and predictive performance.
- Explore the effect of clustering on model quality.

---

## Project Structure

### Part 1 — Core Tasks
- Implement and analyze:
  - K-Means (manual implementation + sklearn)
  - DBSCAN
  - Agglomerative Clustering
  - Gaussian Mixture Models (GMM)
- Evaluate clustering using:
  - Silhouette Score
  - Distortion / Inertia
- Visualize clusters using scatterplots.
- Integrate cluster labels into a Lasso Regression (with MinMaxScaler).
- Compare feature importance and performance before/after clustering.

### Part 2 — Bonus
- Try other supervised models instead of Lasso.
- Optimize hyperparameters (e.g., finding optimal K).
- Combine cluster features from multiple algorithms.
- Experiment with different feature subsets (e.g., bedrooms, bathrooms, interest_level).

---

## Implemented Algorithms

### K-Means (manual implementation)
- Custom centroid initialization
- Iterative update/assignment steps
- Distortion and Silhouette Score computation
- Comparison with sklearn’s KMeans

### DBSCAN
- Parameter exploration: `eps`, `min_samples`
- Outlier detection
- Visualization of arbitrary-shaped clusters

### Agglomerative Clustering
- Sklearn-based implementation
- Multiple distance metrics and linkage types

### Gaussian Mixture Models (GMM)
- EM (Expectation-Maximization) concept demonstration
- Soft clustering via probability distributions

---

## Supervised Learning Integration

Cluster labels are added as new features for a Lasso Regression model.  
The workflow includes:

- Training Lasso with MinMaxScaler
- Measuring predictive performance
- Printing feature weights
- Evaluating how cluster-based features affect the model

---

Clustering was applied on:
- `longitude`, `latitude`
- Optional: `bedrooms`, `bathrooms`, `interest_level`

---

## Evaluation Metrics

- Distortion / Inertia
- Silhouette Coefficient
- Runtime and computational complexity
- Impact on supervised model accuracy

---

## Mandatory Questions (Answered in Notebook)

1. Propose a new centroid initialization method for K-means.  
2. Compare Forgy vs Random Partition vs your method.  
3. Explain how clustering can speed up KNN (hint: kd-tree + clustering).

---

## Tech Stack

- Python 3  
- NumPy, Pandas  
- Scikit-learn  
- Matplotlib, Seaborn  
- Jupyter Notebook  

---

## How to Run

1. Clone the repository.
2. Place datasets in the `data/` directory.
3. Install required dependencies.
4. Run the Jupyter Notebook.
5. Inspect clustering results and model performance.

---