<h3 align="center">DATA MINING</h3>

- - - 

For a reproducible preview &rarr; [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/josepaulosa/Data_Mining/blob/main/Data_Mining.ipynb)
- - - 

> - Data mining is an **`interdisciplinary`** (intersection of machine learning, statistics, and database systems) **field of knowledge**. 
> - Many people treat data mining as a **synonym for knowledge discovery from data**, or **`KDD`**, while others view data mining as **merely** an essential **`step` in the process of KDD** where intelligent methods are applied to **`extract data patterns`**. 
> - As in **industries and in the academic environment** the term data mining is often used to refer to the **`entire knowledge discovery process`** we’ll **adopt this broader view of data mining**.
- - - 
### Dataset:
&rarr; The **unlabeled data is a subset of publicly available** (from https://www.meteoblue.com/) **data about climate in Basel, Switzerland**, which contains 1763 records of data (for 18 features) from the summer and the winter seasons from 2010 to 2019 period and **can be found** [here](https://github.com/josepaulosa/Data_Mining/blob/main/Data.txt)

&rarr; The meaning of each column of data is listed in the notebook.
- - - 
### Tasks:
&rarr; **PRE-PROCESSSING**
- EDA 
    - Descriptive statistics
    - Check if there is any null data
    - Histograms of all features and correlation between all features 
- Feature Selection (considering the conclusions drawn from EDA)
- Standardize 
- Detect and Remove Global Outliers (if < -3 or >3)
- Normalize (to convert to [0, 1])
- Feature Extraction with **`PCA`** (extraction of new, orthogonal - independent - features, which are a linear combination of the original ones)
- PCA Features Contribution to Cumulative Explained Variance 
<br><br>

&rarr; **CLUSTERING**
- **`Silhouette Analysis`** (for finding the optimal number of clusters)
- **`Clustering`** with K-Means and Gaussian Mixture Algorithms
- Choose between K-Means and Gaussian Mixture to Predict the Labels
<br><br>

&rarr; **CLASSIFICATION**
- Classification with K-NN and SVM, using **`Hyperparameter Tuning`** with  **`GridSeachCV`**
- Classification Report
- - - - 
### Achievements:
- Two  **distinct groups of data points** - **clusters** - were **clearly identified within** the **dataset** (**summer** and **winter** days). 
- **Using** the **resulting cluster labels** we **trained 2 classifiers**  using **hyperparameter tuning** with  **GridSeachCV** which allowed us to **reach very high values** for **all considered metrics**.
