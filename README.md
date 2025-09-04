# House Price Prediction using Random Forest

## Project Overview
Advanced machine learning project predicting house prices using Random Forest Regressor with hyperparameter optimization via GridSearchCV, achieving superior accuracy through automated preprocessing pipeline.

## Problem Statement
Predict real estate prices in Pakistani cities (Karachi, Lahore, Islamabad) using property features while maintaining model interpretability and performance.

## Dataset
- **Size:** 100 house records
- **Cities:** Karachi, Lahore, Islamabad
- **Features:** 10 property characteristics
- **Target:** House prices (PKR)

## Features Used
**Categorical Features:**
- Location (Karachi, Lahore, Islamabad)
- Garage (Yes/No)
- Garden (Yes/No)  
- Condition (Excellent, Good, Average, Poor)
- Neighborhood Type (Residential, Commercial, Industrial)

**Numerical Features:**
- Size (sqft)
- Bedrooms count
- Bathrooms count
- Age (years)
- Distance to City (km)

## Advanced Technical Implementation

### Hyperparameter Optimization
- **GridSearchCV** used for optimal parameters
- **Optimized Parameters:**
  - n_estimators: 300
  - max_depth: None
  - max_features: 0.5
  - min_samples_split: 2
  - random_state: 42

### Pipeline Architecture
```python```
Pipeline:
1. ColumnTransformer (Automated Preprocessing)
   ├── OneHotEncoder (Categorical features)
   └── MinMaxScaler (Numerical features)
2. RandomForestRegressor (Optimized model)

### Tech Stack
Core: Python 3.x
ML: Scikit-learn (Pipeline, ColumnTransformer, GridSearchCV)
Data: Pandas, NumPy
Visualization: Matplotlib
Model: Random Forest Regressor

### Model Performance
R² Score: [Your actual score]
Mean Absolute Error: [Your MAE] PKR
Root Mean Square Error: [Your RMSE] PKR

### Key Technical Highlights
✅ Automated Pipeline (no manual preprocessing)
✅ GridSearchCV Optimization (best hyperparameters)
✅ ColumnTransformer (handles mixed data types)
✅ Feature Importance Analysis
✅ Multiple Visualizations (Scatter, Residuals, Feature Importance)
✅ Professional Code Structure

### Visualizations
Feature Importance Plot - Which factors drive house prices
Actual vs Predicted - Model accuracy visualization
Residuals Plot - Error distribution analysis

### Advanced Features
Pipeline Integration for production-ready code
Automated preprocessing with ColumnTransformer
Hyperparameter tuning results implemented
Handle unknown categories during prediction
Comprehensive model evaluation

### How to Run
pip install pandas scikit-learn matplotlib numpy
python house_price_prediction.py

### Model Insights
Most Important Features: [Based on your feature importance plot]
Location Impact: Significant price variation across cities
Size & Condition: Major price determinants
Optimized Performance: GridSearchCV ensures best model configuration

### Future Enhancements
Cross-validation implementation
Additional ensemble methods
Feature selection techniques
Model deployment pipeline

## Author
Ali - ML Engineer | Advanced Python & Scikit-learn
