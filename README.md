# 🌀 DBSCAN Clustering: Income vs Age

## 🧠 Description
This project applies **DBSCAN (Density-Based Spatial Clustering of Applications with Noise)** to segment individuals based on **Age** and **Income($)**.  
DBSCAN can detect clusters of varying shapes and sizes and identify noise (outliers) in the dataset.

---

## 🎯 AIM
To group individuals into clusters using **DBSCAN** and identify potential noise points in the dataset.

---

## 🧩 Goals
- Identify clusters of similar individuals based on **Age** and **Income($)**.  
- Detect **outliers** or noise points automatically.  
- Visualize clusters and noise points using 2D scatter plots.  
- Standardize features using **StandardScaler** for better clustering results.

---

## ⚙️ Technical Details
**Language & Libraries:**  
- Python  
- pandas  
- numpy  
- matplotlib  
- seaborn  
- scikit-learn  

**DBSCAN Parameters Used:**  
- `eps = 0.5` → Maximum distance between two points to be considered neighbors  
- `min_samples = 15` → Minimum number of points required to form a dense region  

---

## 💻 Code Implementation

```python
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns
from sklearn.preprocessing import StandardScaler
```

📊 Results

Number of clusters detected: 0

Number of noise points: 22

All points were considered noise due to high min_samples or sparse distribution in this small dataset.

📋 Observations

DBSCAN did not find any clusters with the current parameters because the dataset is small and sparse.

All data points were treated as noise (-1 label).

Scaling features using StandardScaler ensures distance metrics are comparable.

DBSCAN is sensitive to eps and min_samples — tuning these parameters is crucial for meaningful clusters.


from sklearn.cluster import DBSCAN

