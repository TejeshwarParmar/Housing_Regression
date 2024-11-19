Housing Price Prediction Model
Project Overview
This project implements a machine learning pipeline for predicting median house values using advanced data preprocessing and a Random Forest Regressor.
Key Features

Stratified sampling for robust dataset splitting
Advanced feature engineering
Custom transformers for feature enhancement
Hyperparameter tuning using RandomizedSearchCV
Cluster similarity transformation
Comprehensive preprocessing pipeline

Data Preprocessing

Automatic feature creation (rooms per house, bedrooms ratio, people per house)
Log transformation for selected numerical features
One-hot encoding for categorical features
Cluster similarity for geographical features

Model Details

Algorithm: Random Forest Regressor
Preprocessing: Multi-stage pipeline with custom transformers
Hyperparameter Tuning: RandomizedSearchCV with cross-validation

Performance

Evaluation Metric: Root Mean Squared Error (RMSE)
Confidence Interval: 95% confidence level for error estimation

Key Dependencies

NumPy
Pandas
Scikit-learn
SciPy

Key Preprocessing Steps

Stratified sampling based on income categories
Feature engineering with custom transformers
Advanced preprocessing including:

Imputation
Scaling
Log transformations
Cluster-based feature generation



Hyperparameter Optimization

Randomized search over:

Number of clusters
Maximum features in Random Forest



Usage
Requires Python 3.7+ with scientific computing libraries installed. Download the housing dataset or use the built-in data loading function.
Model Insights
The pipeline identifies the most important features for house value prediction, providing interpretability alongside predictive power.
