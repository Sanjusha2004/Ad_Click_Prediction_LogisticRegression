# Predicting Ad Click Behavior Using Logistic **Regression**

This project uses a synthetic advertising dataset to build a machine learning model that predicts whether a user will click on an online advertisement based on their demographics and internet usage behavior.

---

## Project Type
**Binary Classification** using **Logistic Regression**

---

## Goal

To build a machine learning model that:
- Predicts whether a particular internet user will click on an advertisement.
- Uses features such as age, gender, time spent on site, income, and internet usage.

---

## Dataset Features

The dataset contains the following columns:

- `Daily Time Spent on Site`: Time spent on website (minutes)
- `Age`: Customer's age
- `Area Income`: Average income of the area
- `Daily Internet Usage`: Internet usage per day (minutes)
- `Ad Topic Line`: Title of the ad
- `City`, `Country`: Demographics
- `Male`: Gender (1 = Male, 0 = Female)
- `Timestamp`: Date & time of user activity
- `Clicked on Ad`: Target label (1 = Clicked, 0 = Not Clicked)

---

## Machine Learning Pipeline

- Data Cleaning & Exploration (EDA)
- Visualizations using Matplotlib & Seaborn
- Feature selection
- Train-test split (67/33)
- Logistic Regression Model
- Evaluation: Classification Report, Confusion Matrix, ROC Curve
- Feature Importance Plot
- Model saved using `joblib` and `pickle`

---

## Model Performance

**Classification Report:**

| Metric      | Class 0 (Not Clicked) | Class 1 (Clicked) |
|-------------|------------------------|-------------------|
| Precision   | 0.86                   | 0.95              |
| Recall      | 0.96                   | 0.85              |
| F1-score    | 0.91                   | 0.90              |
| Accuracy    | **0.90** overall       |                   |

**AUC Score (ROC Curve):** `0.96`

---

## Visualizations Included

- Age Distribution
- Area Income vs Age (Jointplot)
- Pairplot (with hue = Clicked on Ad)
- Confusion Matrix (Heatmap)
- ROC Curve
- Sigmoid Curve (Age vs Click Probability)
