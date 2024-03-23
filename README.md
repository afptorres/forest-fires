# Forest Fires
Project developed in the context of the course: Data Mining I. 
The goal was to build a Machine Learning model to predict if a forest fire was intentional (or not).
The data used comprises observations based on fires occured in Portugal between the years 2014 and 2015.

## Motivation

## Problem

## Task 1: Data Understanding and Preparation

The notebooks 'data_preparation.nb.html' and 'data_understanding.nb.html' provide the code used to complete this task and its outputs.

In this task, we had to deal with some quality issues, like inconsistencies and missing values. We also created new features by fetching climate information, relating to temperature and wind, and eliminated others.

Aditionally, we performed data transformation techniques.

We also provide some visualizations, useful for the understanding of the data.

## Task 2: Predictive Modelling

The notebook 'predictive_modelling.nb.html' provides the code used to complete this task and its outputs.

The evaluation metric used was AUC (Area under the Curve). We splitted the data into Train and Test (70% - 30%), and used k-fold Cross Validation, within the Train data.

We also applied recipes resulting in more pre-processing steps:
- Too Disperse predictors -> removed
- Categorical predictors -> converted to numeric values
- Numeric predictors -> centered and scaled
- Date predictors -> sometimes included (depends on the model)
- Variables with large correlations to others -> removed

We considered the following ML models:
- Logistic Regression
- Decision Trees CART
- K-Nearest Neighbors
- Neural Network
- Naive Bayes
- Random Forest
- Boosted Trees

We also performed hypermarameter tuning, in order to achieve the best results.

## Task 3: Kaggle Competition

The file 'deliverables/submission.csv' was produced to submit to the competition. Its creation is described in 'predictive_modelling.nb.html'.

## Results

A presentation 'deliverables/presentation.ppt' was created to expand on some of the process and to explain the results achieved.

The decision of the best model was based on the evaluation of the AUC_ROC metric. We achieved the higher result with Random Forest (0.7627880 in the test portion).

Our team achieved 3rd place, with a total of 14 participant teams, in the Kaggle competition.
