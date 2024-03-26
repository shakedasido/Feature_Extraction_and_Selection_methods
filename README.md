# Covertype Dataset: Dimensionality Reduction (Feature Extraction) and Feature Selection

This project explores various techniques for analyzing and classifying the UCI Machine Learning Repository's Covertype dataset using Jupyter Notebooks. Here, we compare the performance of PCA, LDA, RFE and F1-score methods using K-Nearest Neighbors (KNN) classification.

The comparison is done as follows:

1. I transformed the data in the Covertype dataset using Principal Component Analysis (PCA) and Linear Discriminant Analysis (LDA) for dimensionality reduced (Feature extraction comparison).
2. I selected data with feature selection from the Covertype dataset using Recursive Feature Elimination (RFE) and F-classif (SelectKBest) 

I wrote these two parts in Python, and covered in a separate Jupyter Notebook for each comparison.  

To evaluate the efficiancy of each method that I used for feature extraction and feature selection, I used the same method of classification on them and run the classification report, accuracy, time efficiency checks on them.

**Requirements**

* Python (version 3.6 or later): [https://www.python.org/downloads/](https://www.python.org/downloads/)
* Jupyter:  
  Open a project in a python soporter IDE such as pycharm / VSCode, that will contains this project pages, and use the chosen IDE's terminal to run your commands:
  * For **Notebook** version, Install using:
    * `pip install jupyter`  
  * For the **Lab** version, Install using:
    * `pip install jupyterlab`
  
  A window will open in your home browser where it will be possible to run the code and also create new documents as you wish. For more instructions: [https://jupyter.org/](https://jupyter.org/).  
* Required libraries:
    * NumPy ([https://numpy.org/](https://numpy.org/))
    * Matplotlib ([https://matplotlib.org/](https://matplotlib.org/))
    * scikit-learn ([https://scikit-learn.org/](https://scikit-learn.org/))
        * `sklearn.datasets` for loading the Covertype dataset
        * `sklearn.decomposition` for PCA (covered in a separate notebook)
        * `sklearn.discriminant_analysis` for LDA (covered in a separate notebook)
        * `sklearn.model_selection` for data splitting
        * `sklearn.neighbors` for KNN classification
        * `sklearn.metrics` for confusion matrix and classification report
        * `sklearn.feature_selection` for RFE and SelectKBest (used in this notebook)
    * Seaborn ([https://seaborn.pydata.org/](https://seaborn.pydata.org/))

**Usage**

1. Clone this repository:

   ```bash
   git clone https://github.com/shakedasido/Feature_Extraction_and_Selection_methods
   ```

2. Launch Jupyter Notebook OR Jupyter Lab:

   Jupyter Notebook:

   ```bash
   jupyter notebook
   ```

   Jupyter Lab:


   ```bash
   jupyter lab
   ```

4. Open the Jupyter Notebppk files (`.ipynb` extension) at the chosen enviroment, one by one, and execute the code cells (typically by pressing `Shift+Enter`). These notebooks guide you through the analysis steps:
    * **Data Loading and Preprocessing**
    * **Feature Selection with RFE and F-classif (SelectKBest) and Feature Extraction with PCA and LDA** (each covered in a separate notebook)
    * **Classification with KNN**
    * **Evaluation with Time efficiency, Confusion Matrix and Classification Report**

**Results**

The notebooks will display confusion matrices and classification reports for various approaches, allowing you to compare their impact after KNN performance. You'll also see the time taken for different feature selection and feature extraction methods. 

**Additional Notes**

* This project assumes the Covertype dataset has 7 unique classes.
* The code utilizes KNN with `n_neighbors=5` as a starting point. You can experiment with different values to potentially improve performance.

Enjoy exploring the project and feel free to ask questions about it through its comments! 
