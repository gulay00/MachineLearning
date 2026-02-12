# 🚗 Turbo.az Car Price Prediction

This project builds a machine learning model to predict car prices based on vehicle features scraped from Turbo.az listings.

## 📌 Project Goal
The goal is to estimate vehicle prices using machine learning and evaluate how well different car attributes explain price variation.

## 📊 Dataset
The dataset contains car listings with features such as:

- Brand and model
- Production year
- Engine characteristics
- Mileage
- Region
- Fuel type
- Vehicle type
- Additional sale options (barter, credit, etc.)
- Price (target variable)

## ⚙️ Data Preprocessing
The following preprocessing steps were applied:

- Cleaning inconsistent values
- Handling missing values
- Feature engineering and column cleaning
- Numeric feature scaling using StandardScaler
- Categorical feature encoding using OneHotEncoder
- Train-test split

A preprocessing pipeline was built using `ColumnTransformer` and `Pipeline`.

## 🤖 Model
An **XGBoost Regressor** model was trained to predict vehicle prices.

### Model parameters
- n_estimators = 500
- learning_rate = 0.05
- max_depth = 6
- subsample = 0.8
- colsample_bytree = 0.8

## 📈 Results
Model performance on the test set:

- R² Score: **0.96**
- MAE: ~6,100 AZN
- RMSE: ~9,950 AZN

The model generalizes well with minimal overfitting.

## 🔍 Feature Importance
Feature importance analysis shows which vehicle characteristics most influence price prediction.

## 🛠 Technologies Used
- Python
- Pandas & NumPy
- Scikit-learn
- XGBoost
- Matplotlib

## 🚀 Future Improvements
Possible improvements include:

- Hyperparameter tuning
- Outlier handling
- Additional feature engineering
- Model comparison with other algorithms

## 📎 Usage
Run the notebook:

```bash
jupyter notebook


Data Set:
https://www.kaggle.com/datasets/sehriyarmemmedli/turboaz-cars-project
