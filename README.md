# CS 4412 Data Mining Project
## Pattern Discovery in the Global Terrorism Database (M4 Final)

### Author
Daniel Berezovsky  
CS 4412 – Data Mining  

---

## Project Overview

This project analyzes patterns in the Global Terrorism Database (GTD) using data mining techniques with a focus on **pattern discovery rather than prediction**. The goal is to identify meaningful structure in terrorist incidents through clustering, dimensionality reduction, and interpretable analysis.

To improve consistency and focus on modern terrorism trends, the dataset is restricted to incidents from **2000 onward**.

---

## Discovery Questions

1. Are there natural clusters of terrorist incidents based on attack characteristics?  
2. How do geographic and temporal context affect the clustering structure?  
3. What additional structure appears when a density-based clustering method is used?  

---

## Dataset

**Dataset:** Global Terrorism Database (GTD)  
**Source:** START / Kaggle  

The dataset includes:
- year of incident  
- country and region  
- attack type  
- target type  
- weapon type  
- number killed  
- number wounded  

---

## Techniques Used

### Exploratory Data Analysis
- trends over time  
- geographic concentration  
- attack and weapon distributions  
- casualty severity patterns  

### Clustering
- **K-Means** (primary clustering method)  
- **DBSCAN** (density-based clustering for alternative structure)  

### Dimensionality Reduction
- **PCA** (used for visualization and preprocessing for DBSCAN)  

### Evaluation
- Elbow Method  
- Silhouette Score  

### Interpretation Enhancement
- **Decision Tree** used to explain cluster structure  

---

## Key Findings

- K-Means identifies **three interpretable clusters**
- Silhouette scores do **not peak at k = 3**, but k = 3 is chosen for interpretability
- PCA visualization provides a **rough projection** of clusters (low variance captured)
- DBSCAN does **not produce clean clusters**, instead fragmenting the data into many small groups
- Decision tree reveals which features differentiate clusters

### Named Clusters

- **Cluster 0:** Bombing/Explosive Attacks in Middle East & North Africa  
- **Cluster 1:** Unarmed / Military-Targeted Incidents  
- **Cluster 2:** Armed Assaults in South Asia  

These labels are based on dominant features in each cluster and help translate numerical clusters into meaningful real-world patterns.

---

## Project Structure

```
CS4412Project
│── data/
│   └──globalterrorismdb_0718dist.csv.zip
├── notebooks/
│   └── gtd_m4_polished_final.ipynb
├── docs/
│   └── CS4412_Daniel_Berezovsky_M4_Final_Report.pdf
│   └── GTD_Project_Presentation_M4_Daniel_Berezovsky.pptx
└── README.md
```

---

## How to Run

### 1. Install dependencies
```
pip install pandas numpy matplotlib seaborn scikit-learn
```

### 2. Launch Jupyter
```
jupyter notebook
```

### 3. Open the notebook and run all cells

---

## Dataset Setup (Important)

Place the dataset file:

```
globalterrorismdb_0718dist.csv
```

in the **same directory as the notebook** before running.

---

## Reproducibility Notes

- Random seeds are fixed where applicable  
- Sampling is used for large computations (silhouette + DBSCAN)  
- Notebook runs end-to-end and reproduces all results  

---

## Limitations

- High-dimensional categorical data leads to sparse feature space  
- PCA visualization captures limited variance (~10% in 2D)  
- DBSCAN results are sensitive to parameter choice  
- Clustering results depend on feature engineering decisions  

---

## M4 Improvements

- Corrected silhouette interpretation  
- Added cluster naming  
- Improved PCA and DBSCAN explanations  
- Added decision tree feature labeling  
- Enhanced visualization clarity (optional version)  

---

## Notes

This project was completed as part of **CS 4412 Data Mining**.
