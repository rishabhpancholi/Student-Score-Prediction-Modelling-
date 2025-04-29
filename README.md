# Student Score Prediction Modeling

This project focuses on predicting student academic performance using machine learning models. The analysis and modeling are implemented in a Jupyter notebook (`Model-Training.ipynb`).

## Dataset Overview

The dataset (`stud.csv`) contains information about students' academic performance along with various demographic and educational factors. The dataset includes the following features:

- **Demographic Information:**
  - `gender`: Student's gender
  - `race_ethnicity`: Student's racial/ethnic group (group A, B, C, D, E)
  - `parental_level_of_education`: Education level of parents
  - `lunch`: Type of lunch program (standard/free or reduced)

- **Academic Factors:**
  - `test_preparation_course`: Whether the student completed a test preparation course
  - `math_score`: Score in mathematics
  - `reading_score`: Score in reading
  - `writing_score`: Score in writing

## Target Variable

The project focuses on predicting the `writing_score` as the target variable. The model uses all other features (demographic information, math_score, reading_score, and other academic factors) as input variables to predict a student's writing score.

## Modeling Approach

The project implements various machine learning models to predict student scores, including:

1. **Regression Models:**
   - Linear Regression
   - Ridge Regression
   - Lasso Regression

2. **Tree-based Models:**
   - Decision Tree Regressor
   - Random Forest Regressor
   - XGBoost Regressor
   - AdaBoost Regressor

3. **Nearest Neighbors:**
   - K-Nearest Neighbors Regressor

The modeling process includes:
- Data preprocessing and feature engineering
- Model training and evaluation
- Hyperparameter tuning using GridSearchCV and RandomizedSearchCV
- Performance evaluation using metrics like R² score, Mean Squared Error, and Mean Absolute Error

## Regression Analysis

The project includes comprehensive regression analysis using:
- **Regression Plots (regplot):** Visual representation of the relationship between features and the writing score
- **Coefficient Interpretation:**
  - Positive coefficients indicate a positive relationship with the writing score
  - Negative coefficients indicate a negative relationship with the writing score
  - The magnitude of coefficients shows the strength of the relationship
  - Feature importance is determined by the absolute value of coefficients

## Dependencies

The project uses the following Python libraries:
- NumPy
- Pandas
- Scikit-learn
- XGBoost

## Usage

1. Ensure all dependencies are installed
2. Open and run the `Model-Training.ipynb` notebook
3. The notebook contains all the necessary code for data analysis, model training, and evaluation

## Results

The notebook includes comprehensive analysis of model performance and visualizations to understand the relationships between different features and writing scores. The regression analysis provides insights into:
- Which factors most strongly influence writing performance
- The direction and magnitude of relationships between features and writing scores
- Feature importance rankings for predicting writing scores