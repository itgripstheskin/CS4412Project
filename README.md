# **CS4412 Data Mining Project**

Pattern Discovery in the Global Terrorism Database

Author

Daniel Berezovsky

CS 4412 Data Mining

Kennesaw State University

\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_

### Project Overview

This project explores patterns and relationships within the Global Terrorism Database (GTD) using data mining techniques. The goal is to identify meaningful structures and insights in historical terrorism data through exploratory analysis and unsupervised learning methods.

Rather than focusing on prediction accuracy, the project emphasizes pattern discovery, clustering, and exploratory visualization to better understand global terrorism trends.

\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_

### Dataset

Dataset: Global Terrorism Database (GTD)

Source: https://www.kaggle.com/datasets

The Global Terrorism Database is a comprehensive open-source dataset containing information on terrorist events around the world.

Dataset Characteristics

###### • Events from 1970–present

###### • Includes information such as:

o Year and location of attack

o Attack type

o Weapon type

o Target category

o Number of casualties

o Terrorist group involved

The dataset contains thousands of recorded incidents, making it suitable for large-scale exploratory analysis.

\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_

### Discovery Questions

This project investigates the following discovery-oriented questions:

1.Are there natural clusters of terrorist incidents based on attack characteristics?

2.Which attack types and weapon types frequently occur together?

3.What temporal or geographic patterns exist within the dataset?

These questions aim to uncover underlying structures within the data rather than predicting future events.

\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_

### Techniques Used

The following data mining techniques are applied:

Exploratory Data Analysis (EDA)

•Distribution analysis

•Temporal trends

•Geographic exploration

•Feature relationships

Clustering

•K-Means Clustering

•Identification of natural groupings in attack patterns

Visualization

•Matplotlib

•Seaborn

•Scatter plots and distribution charts

These techniques help reveal patterns, anomalies, and relationships within the data.

\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_

Project Structure

cs4412-project

│

├── data

│   └── dataset files

│

├── notebooks

│   └── Jupyter notebooks for analysis

│

├── src

│   └── Python scripts

│

├── docs

│   └── project proposal and documentation

│

└── README.md

\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_

Tools \& Libraries

Python libraries used in this project include:

• pandas

• numpy

• scikit-learn

• matplotlib

• seaborn

• jupyter notebook

\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_

How to Run the Project

1. Clone the repository:

git clone https://github.com/yourusername/cs4412-project.git

2\. Navigate into the folder:

cd cs4412-project

3\. Install dependencies:

pip install pandas numpy matplotlib seaborn scikit-learn

4\. Launch Jupyter Notebook:

jupyter notebook

5\. Open the notebook inside the notebooks/ folder and run all cells.

\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_

Future Work

Planned future enhancements include:

• Association rule mining - Apriori (or FP-Growth)

• Additional clustering algorithms (DBSCAN or hierarchical clustering)

• Dimensionality reduction techniques such as PCA

• More advanced visualization of discovered patterns

\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_

License

This project is created for educational purposes as part of the CS4412 Data Mining at Kennesaw State University.

