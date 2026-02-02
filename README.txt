TMDB Movie Rating Prediction

This project analyzes and predicts movie ratings using the TMDB 5000 Movies Dataset  
It applies data cleaning, feature engineering, visualization, and multiple regression models to compare performance.

---

Project Overview
The goal of this project is to:
- Explore movie data and understand factors affecting ratings
- Perform data preprocessing and feature engineering
- Train and compare different regression models
- Evaluate model performance using MSE and R²

---

Technologies Used
- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn

---

Dataset
- Dataset: tmdb_5000_movies.csv
- Source: TMDB (The Movie Database) - Kaggle
- Target Variable: Movie Rating (`vote_average`)

---

Data Preprocessing
- Dropped irrelevant columns (homepage, overview, keywords, etc.)
- Extracted:
  - Main genre from `genres`
  - Production country
  - Release year from `release_date`
- Handled missing values:
  - Categorical → `"Unknown"`
  - Numerical → `0`
- Removed outliers using IQR method
- Applied One-Hot Encoding for categorical features
- Standardized numerical features using StandardScaler

---

Exploratory Data Analysis (EDA)
- Boxplots for numerical features
- Average rating per genre
- Rating trends over years
- Correlation heatmap

---

Models Used
1. Linear Regression
2. Polynomial Regression (degree = 2)
3. K-Nearest Neighbors Regressor (KNN)

---

Model Evaluation
Models were evaluated using:
- Mean Squared Error (MSE)
- R² Score

A comparison bar chart was created to visualize model performance.

---

Results
- Polynomial Regression captured non-linear relationships better
- KNN showed competitive performance after feature scaling
- Linear Regression served as a strong baseline model

---

Conclusion
This project demonstrates a complete machine learning pipeline:
from raw data cleaning and visualization to model training and evaluation.

---

Future Improvements
- Hyperparameter tuning (GridSearchCV)
- Try advanced models (Random Forest, XGBoost)
- Feature selection to reduce dimensionality

---

Author
Rahma Magdy
Computer Science Student | Machine Learning Enthusiast
