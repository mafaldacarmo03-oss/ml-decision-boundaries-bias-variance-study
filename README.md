# Decision Boundaries & Bias-Variance Study

## Project Overview

This project investigates how different machine learning algorithms behave under varying data distributions and complexity levels. Through a combination of synthetic classification problems and real-world data, the study explores:

- Decision boundary formation
- Model assumptions and limitations
- Class imbalance effects
- Non-linear separability
- The bias-variance trade-off

The project was developed within the Master's Degree in Computational Statistics and Data Analysis.
The notebook contains critical analyses and interpretations of the results written in Portuguese.

---

## Objectives

The main goals of this study are:

- Compare the behavior of different classification algorithms under diverse geometric data structures.
- Analyze the impact of balanced and imbalanced class distributions.
- Investigate how model assumptions influence performance.
- Empirically study the bias-variance trade-off using real-world data.
- Develop intuition about overfitting, underfitting, and model complexity.

---

## Synthetic Classification Datasets

Several artificial datasets were generated to challenge different model assumptions.

| Dataset | Description |
|----------|-------------|
| Headlights | Two partially overlapping Gaussian blobs |
| Shell | Circular blob versus a thin rectangular strip |
| DD | Two semi-circular "D-shaped" distributions |
| XOR | Classic non-linearly separable problem |
| Chess4 | Alternating class pattern on a 4×4 grid |
| Roseta2 | Central cluster surrounded by a ring |
| Roseta3 | Multiple concentric alternating rings |

Each dataset was evaluated under:

- Balanced classes (50/50)
- Imbalanced classes (90/10)

---

## Models Evaluated

### Instance-Based Learning

- 1-Nearest Neighbors (1NN)
- 5-Nearest Neighbors (5NN)
- 10-Nearest Neighbors (10NN)

### Linear Models

- Logistic Regression
- Linear Discriminant Analysis (LDA)

### Non-Linear Probabilistic Models

- Quadratic Discriminant Analysis (QDA)

---

## Experimental Framework

For every synthetic dataset:

1. Independent training and testing sets were generated.
2. Models were trained using the training data.
3. Classification accuracy was evaluated on unseen observations.
4. Decision boundaries were visualized and compared.
5. Model rankings were analyzed across scenarios.

---

## Decision Boundary Analysis

The experiments highlight how different algorithms adapt to data geometry.

### Key Observations

- Logistic Regression struggles on highly non-linear structures such as XOR and concentric rings.
- LDA performs well when class distributions satisfy linear Gaussian assumptions.
- QDA captures curved decision boundaries more effectively.
- kNN adapts naturally to complex local structures but may become sensitive to noise and sample density.
- Class imbalance can significantly alter decision regions and predictive performance.

---

## Custom Dataset Design

An additional synthetic dataset was created to intentionally violate specific modeling assumptions.

The goal was to generate scenarios where model rankings differed substantially from previous experiments, emphasizing the relationship between:

- Data geometry
- Noise structure
- Model flexibility
- Generalization ability

---

## Bias-Variance Trade-Off Study

A second part of the project focuses on empirical bias-variance decomposition using the Breast Cancer Wisconsin dataset.

### Models Analyzed

- Decision Trees
- Ensemble Methods
- Support Vector Machines (SVM)
- Multi-Layer Perceptrons (MLP)

### Topics Investigated

- Bias estimation
- Variance estimation
- Total prediction error decomposition
- Overfitting versus underfitting
- Regularization effects
- Complexity control

---

## Results and Insights

The experiments revealed several important machine learning principles:

- Simple linear models fail when decision boundaries are highly non-linear.
- kNN performance depends strongly on neighborhood size and local data structure.
- QDA performs particularly well when quadratic Gaussian assumptions are approximately satisfied.
- Ensemble methods effectively reduce variance while maintaining predictive power.
- Support Vector Machines achieve strong generalization through margin maximization.
- Model complexity must be carefully controlled to balance bias and variance.

---

## Technologies Used

- Python
- NumPy
- SciPy
- scikit-learn
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## Skills Demonstrated

- Machine Learning
- Statistical Learning Theory
- Classification Methods
- Bias-Variance Analysis
- Model Evaluation
- Data Visualization
- Experimental Design
- Python for Data Science

---

## Authors

- Ana Mafalda Araújo do Carmo
- Rafaela Afonso Claro Pinto

## Academic Context

Statistical Learning Models

Faculty of Sciences – University of Porto

Academic Year 2025/2026
