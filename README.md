# 📊 Supercondutivity

## 🗃️ Dataset: UCI Supercoductivity Data
Source: https://archive.ics.uci.edu/dataset/464/superconductivty+data 
Format: CSV
<br />
<br />

## Task 1: Build Supervised Learning Models
In the SLM file the goal was to predict the critical temperature based on the features extracted.

## 🔍 Objectives
### 1: Dimensionality Reduction
### 2: Create a Regression and Classification model 
<br />
<br />

## Task 2: Build Unsupervised Learning Models (Clustering)
In the USLM file the goal was to identify clusters in the data 

Note 1: The last column (material) of the unique_m.csv file is an identifier and should be discarded and not used in the analysis

Note 2 The last column is the Dependent Variable (critical_temp) and should not be used in the analysis, except in Objective 2 

## 🔍 Objectives
### 1: Clustering

Using the data from the train.csv file determine the best clustering approach able to classify this dataset

Using the data from the unique_m.csv file determine the best clustering approach able to classify this dataset
compare both approaches in computational performance and clustering quality (using intrinsic methods)

WARNING: columns may have VERY different ranges. This should be handled adequately

### 2: Evaluating clustering with extrinsic methods

Create the following Classes for the dependent variable (critical_temp):

VeryLow - critical_temp in [0.0, 1.0,[

Low - critical_temp in [1.0, 5.0,[

Medium - critical_temp in [5.0, 20.0,[

High - critical_temp in [20.0, 100.0,[

VeryHigh - critical_temp in >= 100.0

With the clusters produced in objective 2, using extrinsic methods, verify the quality of each model, for both the train.csv and the unique_m.csv clusters

## 🛠️ Tools
- Python (Pandas, NumPy, scikit-learn)
- Jupyter Notebook

## 📈 Methodologies
1. **Processing Data**
2. **Dimensionality Reduction SVD**
4. **Regression and Classificatiom Models**
5. **Discussion**

## 💡 Findings
- Dimensionality Reduction of 167 variables data showed that the first 84 components explains 87% of the data.
- Decision Tree Regressor achieved an EVS of 88.6% using all 167 variables
- An EVS of 86.4% was achieved using only the first 65 components
- Decision Tree Classifier achieved an accuracy of 81%
- Using the first 65 components achieves the same accuracy
- The Classifier have a good performance with much less data
- Gaussian Naive Bayes Classifier showed a poorer performance when compared to Decision Trees.
