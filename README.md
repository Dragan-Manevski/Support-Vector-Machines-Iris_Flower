### --------------------------------------------------------------------------------------------------------
# Support Vector Machines - Iris Flower
### --------------------------------------------------------------------------------------------------------
### Support Vector Machines:
- an **algorithm**:
    - based on **Supervised Learning**
    - to solve **Regression and Classification**
    - where machines **learn with supervision**
    - **input data are labeled** and **expected output data is known**
    - with key **objective**:
      - **to predict (classify) a categorical (qualitative) dependent output value (y)** based on **independent input variable(s) (x)** -> for **Classification problems**
      - **to predict a continuous (quantitative) numeric dependent output value (y)** based on **independent input variable(s) (x)** -> for **Regression problems**
    - where we try:
      - to identify **to which category, the new observation belongs to**
      - to find **the best fit line (equation) that can be used to make predictions**
- **Regression and Classification analysis** are a **predictive modeling techniques**
- The **Support Vector Machines** algorithm **builds a model**:
    - that **assigns new observations into one or other category**
    - where the **observations of the separate categories are divided by clear gap**
      - **new observations are mapped into the same space and predicted to belong to a category** based on which side of the gap they fall on
      - **create and choose** the **hyper-plane (line) that separates the classes the best**:
          - for **linearly separable data** -> use hyper-plane that **maximizes the margin between the classes**
          - for **non-linearly separable data** -> use "kernel trick"
      - **vector point that touch the margin line** are known as **Support Vectors**

### --------------------------------------------------------------------------------------------------------
### Project Objective: Predicting type of Iris Flower
Create a model that allows to put in a few features of Iris Flower and returns back a prediction (classification) of the type of Iris Flower. Information about the Iris flower is in a built-in Iris Flower dataset which is imported from Scikit-Learn datasets (https://scikit-learn.org/stable/modules/generated/sklearn.datasets.load_iris.html).

The Iris Flower dataset is a classic and very easy multi-class classification dataset. The Iris Flower dataset or Fisher's Iris dataset is a multivariate dataset introduced by the British statistician, eugenicist, and biologist Ronald Fisher in his 1936 paper "The use of multiple measurements in taxonomic problems" as an example of linear discriminant analysis. The dataset consists of 50 samples from each of three species of Iris (Iris Setosa, Iris Virginica and Iris Versicolor). Four features were measured from each sample: the length and the width of the sepals and petals, in centimeters, stored in a 150 x 4 numpy.ndarray. Based on the combination of these four features, Fisher developed a linear discriminant model to distinguish the species from each other.

This is a copy of UCI ML Iris Flower recognition dataset: http://archive.ics.uci.edu/ml/datasets/Iris

The Iris Flower dataset contains the following columns:
- **sepal length** in cm
- **sepal width** in cm
- **petal length** in cm
- **petal width** in cm
- **species** - type of Iris Flower
    - class 0 = Iris Setosa
    - class 1 = Iris Versicolour
    - class 2 = Iris Virginica

### --------------------------------------------------------------------------------------------------------
### Table of Contents:
1. File Descriptions
2. Technologies Used
3. Structure of Notebook
4. Executive Summary

#### 1. File Descriptions
- Support Vector Machines - Iris_Flower.ipynb
- README.md

#### 2. Technologies Used
- Python
- Pandas
- Numpy
- Matplotlib
- Seaborn
- Scikit-Learn

#### 3. Structure of Notebook
1. Import the Libraries
2. Load the Data
3. Set up the Data
4. Exploratory Data Analysis
    - 4.1 Check out the Data
    - 4.2 Data Visualization
5. Data Preprocessing and Feature Engineering
    - 5.1 Identify the variables
    - 5.2 Dealing with Missing values
      - 5.2.1 Dealing with Missing values in Columns
      - 5.2.2 Dealing with Missing values in Rows
    - 5.3 Dealing with the Non-numerical features
6. Train and Test the Support Vector Machines model
    - 6.1 Split the columns
    - 6.2 Split the data into Training dataset and Testing dataset
    - 6.3 Create the Support Vector Machines model
    - 6.4 Train / fit the Support Vector Machines model
    - 6.5 Predictions from the model on Testing data
    - 6.6 Evaluate the model on Testing data
      - 6.6.1 Classification report
      - 6.6.2 Confusion matrix
    - 6.7 GridSearchCV
      - 6.7.1 Create the Grid of parameters
      - 6.7.2 Create the GridSearchCV model (Re-create the Support Vector Machines model)
      - 6.7.3 Train / fit the GridSearchCV model (Re-train / Re-fit the Support Vector Machines model)
      - 6.7.4 Predictions from the GridSearchCV model (Re-predictions from the Support Vector Machines model) on Testing data
      - 6.7.5 Evaluate the GridSearchCV model (Re-evaluate the Support Vector Machines model) on Testing data
        - 1. Classification report
        - 2. Confusion matrix

#### 4. Executive Summary
TBA
