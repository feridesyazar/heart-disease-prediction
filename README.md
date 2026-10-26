# ❤️ Heart Disease Prediction

### Machine Learning | Binary Classification

In this project, we explore health measurements to predict the `HeartDisease` label using **Logistic Regression**. We analyze the dataset, prepare the features, train a model, and evaluate its predictions with simple Python code.

## Dataset

- **Source:** [Heart Failure Prediction Dataset – Kaggle](https://www.kaggle.com/datasets/fedesoriano/heart-failure-prediction)
- **File:** `heart.csv`
- **Size:** 918 records, 12 columns
- **Target:** `HeartDisease` (`0` = no recorded heart disease, `1` = heart disease)

The dataset contains features such as age, chest pain type, blood pressure, cholesterol, maximum heart rate, and ECG-related measurements.

## Project Steps

1. **Data Overview:** Read the CSV and inspect the columns
2. **EDA:** Check data types, missing values, and basic statistics
3. **Visualization:** Explore class distribution, maximum heart rate, and correlations
4. **Feature Engineering:** Convert categorical columns using `pd.get_dummies()`
5. **Train/Test Split:** Use 80% for training and 20% for testing, with stratification
6. **Scaling and Modelling:** Fit `StandardScaler` on the training data and train Logistic Regression
7. **Evaluation:** Review Accuracy, Precision, Recall, F1-Score, and the confusion matrix

## Results

| Metric | Test score |
|---|---:|
| Accuracy | 0.886 |
| Precision | 0.872 |
| Recall | 0.931 |
| F1-Score | 0.900 |

These results come from **one 80/20 train/test split** (`random_state=42`). They do not establish clinical performance.


## Limitations

- The dataset has **172 zero values in `Cholesterol`** and **one zero value in `RestingBP`**. These may represent unrecorded measurements; they were not corrected in this beginner project.
- The reported metrics are based on a single test split and may change with different data.

## Data Source

[Fedesoriano – Heart Failure Prediction Dataset (Kaggle)](https://www.kaggle.com/datasets/fedesoriano/heart-failure-prediction)
