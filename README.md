# Housing Price Prediction Model

## Project Overview

This project implements a machine learning pipeline for predicting median house values using advanced data preprocessing and a Random Forest Regressor.

### Key Features:
- **Stratified sampling** for robust dataset splitting.
- **Advanced feature engineering** for enhanced predictive power.
- Custom transformers for feature enhancement.
- **Hyperparameter tuning** using `RandomizedSearchCV`.
- **Cluster similarity transformation** for geographical features.
- Comprehensive **preprocessing pipeline** for cleaning and transformation.

---

## Data Preprocessing

### Automatic Feature Creation:
- **Rooms per house**: `total_rooms` divided by `households`.
- **Bedrooms ratio**: `total_bedrooms` divided by `total_rooms`.
- **People per house**: `population` divided by `households`.

### Transformations:
- **Log transformation** for selected numerical features to reduce skewness.
- **One-hot encoding** for categorical features (e.g., `ocean_proximity`).
- **Cluster similarity** features for geographical data (`latitude`, `longitude`).

---

## Model Details

- **Algorithm**: Random Forest Regressor
- **Preprocessing**: Multi-stage pipeline with custom transformers
- **Hyperparameter Tuning**: `RandomizedSearchCV` with cross-validation for optimal performance.

---

## Performance

- **Evaluation Metric**: Root Mean Squared Error (RMSE)
- **Confidence Interval**: 95% confidence level for error estimation.

---

## Key Dependencies

- `NumPy`
- `Pandas`
- `Scikit-learn`
- `SciPy`

Install these libraries using:
```bash
pip install numpy pandas scikit-learn scipy
