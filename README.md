# Rain Prediction using Logistic Regression

## Project Overview

This project predicts whether it will rain tomorrow using Machine Learning.

The target variable is `RainTomorrow`, which contains two possible values:
- Yes
- No

## Dataset

The dataset contains Australian weather information with 142,193 rows and 24 columns.

The features include:

- Location
- MinTemp
- MaxTemp
- Rainfall
- Evaporation
- Sunshine
- WindGustSpeed
- WindSpeed9am
- WindSpeed3pm
- Humidity9am
- Humidity3pm
- Pressure9am
- Pressure3pm
- Cloud9am
- Cloud3pm
- Temp9am
- Temp3pm
- RainToday
- RISK_MM

The target variable is `RainTomorrow`.

## Machine Learning Workflow

1. Load the dataset
2. Check the shape and columns
3. Check data types
4. Handle missing values
5. Perform Exploratory Data Analysis
6. Separate features (X) and target (y)
7. Encode categorical variables
8. Split the data into training and testing sets
9. Scale the features
10. Train the Logistic Regression model
11. Evaluate the model

## Algorithm Used

### Logistic Regression

Logistic Regression is a classification algorithm used to predict whether it will rain tomorrow or not.

The model predicts two classes:

- `Yes` → Rain tomorrow
- `No` → No rain tomorrow

## Tools and Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## Project File

The complete Jupyter Notebook containing the code and analysis is available in this repository.

## Conclusion

A Logistic Regression model was trained to predict whether it will rain tomorrow based on different weather conditions.
