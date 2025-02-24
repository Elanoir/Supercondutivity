Dataset: UCI Supercoductivity Data

In the SLM file the goal was to predict the critical temperature based on the features extracted.

Task: Build Supervised Learning Models

Objectives: 

1: Dimensionality Reduction

2: Create a Regression and Classification model


In the USLM file the goal was to identify clusters in the data 

Task - Build Unsupervised Learning Models (Clustering)

Note 1: The last column (material) of the unique_m.csv file is an identifier and should be discarded and not used in the analysis

Note 2 The last column is the Dependent Variable (critical_temp) and should not be used in the analysis, except in Objective 2 as described below

Objectives:

1:Clustering

Using the data from the train.csv file determine the best clustering approach able to classify this dataset

Using the data from the unique_m.csv file determine the best clustering approach able to classify this dataset
compare both approaches in computational performance and clustering quality (using intrinsic methods)

WARNING: columns may have VERY different ranges. This should be handled adequately

2: Evaluating clustering with extrinsic methods

Create the following Classes for the dependent variable (critical_temp):

VeryLow - critical_temp in [0.0, 1.0,[

Low - critical_temp in [1.0, 5.0,[

Medium - critical_temp in [5.0, 20.0,[

High - critical_temp in [20.0, 100.0,[

VeryHigh - critical_temp in >= 100.0

With the clusters produced in objective 2, using extrinsic methods, verify the quality of each model, for both the train.csv and the unique_m.csv clusters
Discuss your results and compare them with the results of Objective 1
