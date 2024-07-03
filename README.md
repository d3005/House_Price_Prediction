# House Price Prediction System Using Data Analytics Algorithms
## Introduction
This project involves developing a predictive model to forecast house prices based on various factors. The steps include data collection, preprocessing, feature engineering, model selection, and evaluation. Below is the complete source code and a detailed explanation of each step.

## Data Collection
The dataset used for this project is the [House Prices Dataset](https://www.kaggle.com/c/house-prices-advanced-regression-techniques/data?select=sample_submission.csv)
The dataset contains information about various features of houses such as square footage, number of bedrooms, bathrooms,
and so on. The target variable is the sale price of the house.

## Data Preprocessing
The first step in data preprocessing is to clean the data by removing any missing values or outliers. This
can be done using the pandas library in Python. Next, we need to encode the categorical variables using
one-hot encoding or label encoding. Finally, we need to scale the numerical variables using the MinMax
Scaler from the scikit-learn library.

## Feature Engineering
The next step is to engineer new features from the existing ones. For example, we can create a
new feature that represents the ratio of the square footage to the number of bedrooms. This can help us
understand how the size of the house affects the price.

### Model Selection and Training
1. **Gradient Boosting Regressor**:- Trained using `GradientBoostingRegressor` on the selected features.- Evaluated using Root Mean Squared Error (RMSE).
2. **Linear Regression**:- Trained using `LinearRegression`.- Evaluated using Mean Squared Error (MSE) and R^2 score.
3. **Random Forest Regressor**:- Trained using `RandomForestRegressor`.- Evaluated using Mean Squared Error (MSE) and R^2 score
4. **Support Vector Regressor**:- Trained using `SVR`.- Evaluated using Mean Squared Error (MSE) and R^2 score.

  ### Design Choices- **Gradient Boosting Regressor**: Chosen for its ability to handle non-linear relationships and
 interactions between features.- **Random Forest Regressor**: Chosen for its robustness and ability to handle over fitting by
 averaging multiple decision trees.- **Linear Regression**: Included for comparison as a baseline model

### Model Evaluation
- **Evaluation Metrics**: Used RMSE for Gradient Boosting and MSE, R^2 for Linear Regression and Random Forest.
- **Visualization**: Plotted Actual vs Predicted SalePrice for Random Forest.- Visualized feature importance for Random Forest to understand which features are most influential.

### Design Choices
- **Gradient Boosting Regressor**: Chosen for its ability to handle non-linear relationships and interactions between features.
- **Random Forest Regressor**: Chosen for its robustness and ability to handle overfitting by averaging multiple decision trees.
- **Linear Regression**: Included for comparison as a baseline model.

## Challenges
- **Data Cleaning**: Handling missing values was crucial to avoid biases and ensure model accuracy.
- **Feature Selection**: Selecting the right features without overfitting the model required careful consideration.
- **Model Evaluation**: Choosing appropriate metrics to evaluate and compare models was essential to select the best performing model.

