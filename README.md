# Titanic_space_ship_group_8
 Overview

This project aims to predict whether passengers were transported or not on the fictional spaceship Titanic dataset using various machine learning and deep learning models. We performed detailed data preprocessing, exploratory data analysis (EDA), model training with hyperparameter tuning, SHAP-based interpretability, and result comparison.

# Pre-Processing

Missing Value Handling: Filled missing values using median (for numerical) and mode (for categorical features).
Feature Engineering: Extracted new features like deck, group size, and family indicator.
Categorical Encoding: Used one-hot encoding and label encoding based on model requirements.
Scaling: Applied StandardScaler for models sensitive to feature scales.
Train-Test Split: Split the dataset into training, validation, and test sets.
# Exploratory Data Analysis

Histograms & Box Plots: Visualized distribution and outliers.
Correlation Heatmap: Identified relationships between numerical variables.
PCA (Principal Component Analysis): Reduced dimensionality to understand data variance.
Scatter Plots: Explored relationships between important features.
# Models

Random Forest Classifier
Tuned using GridSearchCV
Best Params: n_estimators=200, max_depth=10, min_samples_split=5, class_weight='balanced'
Accuracy: 79.8%
XGBoost Classifier
Tuned using RandomizedSearchCV
Best Params: max_depth=7, learning_rate=0.05, subsample=0.8, gamma=0.5
Accuracy: 80.0%
Convolutional Neural Network (CNN)
Used 1D CNN with GlobalMaxPooling and dropout
Accuracy: (Your CNN score here, e.g., 77.5%)
# Model Evaluation

Evaluated using Accuracy, Precision, Recall, and F1-score
Used confusion matrix for class-wise prediction analysis
Applied SHAP values to interpret feature importance for tree-based models (Random Forest & XGBoost)
# Submissions

Predictions saved in CSV files:
submission_rf.csv, submission_xgb.csv, submission_cnn.csv
