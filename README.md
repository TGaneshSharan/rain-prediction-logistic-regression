# Rain Prediction Using Logistic Regression

## Project Overview

This project predicts whether it will rain tomorrow using historical weather data from Australia.

The project uses **Logistic Regression**, a supervised machine learning algorithm used for binary classification.

The main objective is to understand the complete machine learning workflow, including data exploration, data preprocessing, feature engineering, model training, and evaluation.

---

## Objective

The objective of this project is to predict the value of **RainTomorrow** as:

- `0` → No Rain
- `1` → Rain

The model learns patterns from historical weather conditions and predicts whether rainfall is expected on the following day.

---

## Dataset

The dataset contains historical weather observations from Australia.

### Dataset Details

- **Total Records:** 66,410
- **Total Features:** 17
- **Target Variable:** `RainTomorrow`
- **Classes:** No / Yes
- **Class Distribution:** Approximately 52% No and 48% Yes

The dataset contains real weather observations, with missing values handled during preprocessing.

---

## Features Used

The following weather-related features were used:

- Date
- Location
- MinTemp
- MaxTemp
- Rainfall
- WindGustDir
- WindGustSpeed
- WindDir9am
- WindDir3pm
- WindSpeed9am
- WindSpeed3pm
- Humidity9am
- Humidity3pm
- Pressure9am
- Pressure3pm
- RainToday

### Target Variable

`RainTomorrow`

- `No` → 0
- `Yes` → 1

---

## Data Preprocessing

The following preprocessing steps were performed:

1. Loaded the dataset using Pandas.
2. Checked the structure and data types.
3. Checked missing values.
4. Checked duplicate records.
5. Converted the `Date` column into:
   - Year
   - Month
   - Day
6. Removed the original `Date` column after feature extraction.
7. Converted the target variable into binary values.
8. Split the dataset into training and testing sets.
9. Filled missing numerical values using the mean.
10. Filled missing categorical values using the mode.
11. Converted categorical variables into numerical form using one-hot encoding.
12. Checked for outliers using the IQR method.
13. Standardized features using `StandardScaler`.

---

## Exploratory Data Analysis

Exploratory Data Analysis was performed to understand:

- Dataset structure
- Missing values
- Target variable distribution
- Numerical feature statistics
- Duplicate records
- Outliers
- Rainfall-related patterns

Visualizations were created using Matplotlib and Seaborn.

---

## Machine Learning Model

### Logistic Regression

Logistic Regression was selected because the target variable contains two classes:

- No Rain
- Rain

The model was trained using the preprocessed training data and evaluated on unseen test data.

---

## Model Evaluation

The model was evaluated using:

- Accuracy
- Precision
- Recall
- F1 Score
- ROC-AUC

### Results

| Metric | Score |
|---|---:|
| Accuracy | 77.96% |
| Precision | 78.88% |
| Recall | 73.87% |
| F1 Score | 76.29% |
| ROC-AUC | 86.36% |

---

## Conclusion

The Logistic Regression model achieved an accuracy of approximately **77.96%** on the test data.

The ROC-AUC score of **86.36%** indicates that the model has a good ability to distinguish between rainy and non-rainy days.

This project demonstrates the complete workflow of a binary classification problem, from data preprocessing and exploratory data analysis to machine learning model training and evaluation.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

---

## Project Structure

```text
rain-prediction-logistic-regression/
│
├── README.md
├── weatherAUS_reduced_columns_52_48.csv
└── weather_prediction_logistic_regression.ipynbin tomorrow based on different weather conditions.
