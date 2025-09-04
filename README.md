# house-price-prediction-king-county
A machine learning model to predict house prices in King County, WA, achieving 90% accuracy (R²) using multiple regression models. The dataset was obtained from Kaggle and contains over 21,000 house sale records with features such as bedrooms, bathrooms, square footage, condition, and location (zipcode).
The goal of this project was to build and compare different regression models to predict house prices.

Steps followed:

Data Collection 

Data Preprocessing

Handled missing values

Scaled numerical features

Encoded categorical features (zipcode) using one-hot encoding

Model Training – Split the dataset into train/test sets and trained multiple models.

Model Evaluation – Compared results using R² score and selected the best model.

Model	R² Score
Multiple Linear Regression (R² = 0.81): Captures linear relationships but limited for complex patterns.
Decision Tree Regression (R² = 0.80): Easy to interpret but tends to overfit.
Random Forest (R² = 0.88): Reduces overfitting and improves accuracy by averaging multiple trees.
SVR (R² = 0.85): Works well for smaller datasets with clear margins but sensitive to scaling.
XGBoost (R² = 0.90): Most powerful, handles non-linearities, and produced the best results.

Best Model: XGBoost with R² = 0.92
XGBoost was chosen because it provided the most accurate and reliable predictions on unseen data.

Used :
Python
Pandas, NumPy
Matplotlib, 
Scikit-learn
XGBoost

Key Learnings

Applied data preprocessing techniques such as scaling and one-hot encoding.
Gained experience comparing multiple regression algorithms.
Learned how to evaluate models using R² score, MSE, and MAE.
Identified XGBoost as the best model for structured tabular data in this project.

Next Steps

Improve feature engineering for better predictions.
Deploy the model using Flask/Streamlit for real-world usage.
Try ensemble stacking of multiple models.
Author: Mostafa Amr
