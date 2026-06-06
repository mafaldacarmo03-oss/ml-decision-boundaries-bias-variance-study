# Decision Boundaries & Bias-Variance Study

## Overview

This project explores the behavior of different machine learning models through synthetic datasets and real-world data. The focus is on understanding decision boundaries, model assumptions, and the bias-variance trade-off.
The study combines classification experiments on artificial datasets with an empirical analysis of bias and variance using the Breast Cancer Wisconsin dataset.

## Objectives

- Analyze how different ML algorithms behave under varying data distributions
- Compare decision boundaries across models
- Study the impact of class imbalance and geometry on classification performance
- Investigate the bias-variance trade-off in classical and modern ML models
- Visualize and interpret model behavior empirically

## Synthetic Datasets

The following datasets were generated to test model assumptions:

Headlights: two overlapping Gaussian blobs
Shell: circular blob vs thin rectangular strip
DD: two “D-shaped” semi-circular distributions
XOR: classic non-linear separability problem
Chess4: 4x4 grid alternating classes
Roseta2: central blob + surrounding ring
Roseta3: multiple concentric alternating rings

Each dataset was tested under:

Balanced classes (50/50)
Unbalanced classes (90/10)

## Machine Learning Models

The following classifiers were evaluated:

k-Nearest Neighbors (1NN, 5NN, 10NN)
Logistic Regression
Linear Discriminant Analysis (LDA)
Quadratic Discriminant Analysis (QDA)


## Experiments

1. Classification Performance

For each dataset:

Models were trained and tested on independent sets
Accuracy was computed
Models were ranked based on performance

2. Analysis of Results

Results were interpreted based on:

Model assumptions (linearity, Gaussianity, locality)
Data geometry and separability
Sensitivity to class imbalance

Simple models (e.g., logistic regression) fail on highly non-linear datasets
kNN is highly sensitive to local structure and noise
QDA performs well when Gaussian assumptions hold

3. Additional Dataset

(foi proposto um novo dataset com propriedades que permitissem apresentar resultados diferentes)
A custom dataset was designed to highlight differences in model rankings by breaking specific assumptions (e.g., non-linearity or high noise).


# Bias-Variance Study
Using the Breast Cancer Wisconsin dataset:

Models analyzed

Decision Trees
Ensemble methods
Support Vector Machines (SVM)
Multi-Layer Perceptrons (MLP)


# Focus

Empirical bias-variance decomposition
Effect of model complexity
Overfitting vs underfitting behavior
Regularization and variance control techniques


# Visualizations

Bias vs variance plots
Total error decomposition
Model comparison under different configurations


# Key Insights
Simple models (e.g., logistic regression) fail on highly non-linear datasets
kNN is highly sensitive to local structure and noise
QDA performs well when Gaussian assumptions hold
Ensembles and SVMs reduce variance effectively
Bias-variance trade-off can be controlled via model complexity and regularization


# Tools Used

Python
NumPy, SciPy
scikit-learn
Matplotlib / Seaborn


# Authors

Ana Mafalda Araújo do Carmo
Rafaela Afonso Claro Pinto
