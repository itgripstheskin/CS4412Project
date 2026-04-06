# CS 4412 Data Mining Project
## Pattern Discovery in the Global Terrorism Database

### Author
Daniel Berezovsky  
CS 4412 – Data Mining  

---

## Project Overview

This project analyzes patterns in the Global Terrorism Database (GTD) using data mining techniques with a focus on **pattern discovery** rather than prediction. The goal is to identify meaningful structure in terrorist incidents by combining exploratory data analysis, clustering, dimensionality reduction, and interpretable rule-based explanation.

To improve consistency and focus on modern terrorism trends, the analysis is restricted to incidents from **2000 onward**.

---

## Discovery Questions

1. Are there natural clusters of terrorist incidents based on attack characteristics?
2. How do geographic and temporal context affect the clustering structure?
3. What additional structure appears when a density-based clustering method is used?

---

## Dataset

**Dataset:** Global Terrorism Database (GTD)  
**Source:** Kaggle / START-UMD Global Terrorism Database  

The GTD contains worldwide terrorist incident records with attributes such as:

- year of incident
- country and region
- attack type
- target type
- weapon type
- number killed
- number wounded

For this project, the most relevant features include attack type, target type, weapon type, region, year, and a derived casualty measure.

---

## Techniques Used

### Exploratory Data Analysis
- attacks per year
- top countries by incident count
- attack type distributions
- weapon type distributions
- casualty distributions
- severity comparisons across attack types

### Clustering
- **K-Means** for broad segmentation of incidents
- **DBSCAN** for density-based grouping and detection of unusual cases

### Dimensionality Reduction
- **PCA** for lower-dimensional visualization and preprocessing for DBSCAN

### Evaluation
- **Elbow Method**
- **Silhouette Score**

### Interpretation Enhancement
- **Decision Tree** used to explain cluster structure with interpretable rules

---

## Key M3 Improvements

This version expands the earlier clustering work by:

- adding silhouette score analysis to support cluster selection
- using one-hot encoding for categorical features
- incorporating **region** and **year** into the feature set
- replacing a simple 2D scatter view with **PCA-based visualization**
- adding **DBSCAN** as a second clustering method
- using a **decision tree** to explain how clusters are distinguished

---

## Results Summary

- K-Means identifies **three broad clusters** of terrorist incidents
- silhouette scoring supports the choice of **k = 3**
- PCA provides a more meaningful visualization of cluster separation
- DBSCAN identifies dense regions and noise points, highlighting less typical incidents
- decision tree rules make cluster membership easier to interpret

Together, these methods suggest that terrorist incidents are not homogeneous. They differ in terms of severity, tactics, weapons, targets, regional context, and time period.

---

## Project Structure

```text
cs4412-project
│
├── data/
│   └── dataset file or access instructions
├── notebooks/
│   └── gtd_m3_analysis.ipynb
├── docs/
│   └── M3_Final_Expanded_Report_v2.pdf
└── README.md
```

---

## How to Run

1. Install dependencies:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

2. Launch Jupyter Notebook:

```bash
jupyter notebook
```

3. Open the notebook in the `notebooks/` folder and run all cells.

4. Make sure the GTD CSV file is in the expected location before running the notebook.

---

## Reproducibility Notes

- The analysis uses fixed random seeds where relevant for reproducibility.
- Some steps such as silhouette scoring and DBSCAN use sampling to keep runtime manageable on a large dataset.
- The notebook is designed to run end-to-end and reproduce the main results shown in the report.

---

## M4 Plan

Future polish will focus on:

- refining cluster names and interpretations
- improving visual presentation
- strengthening the limitations discussion
- tightening the final narrative of findings

---

## Notes

This project was created for academic purposes as part of **CS 4412 Data Mining**.
