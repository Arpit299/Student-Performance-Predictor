# Student Performance Predictor

This project implements a machine learning pipeline to predict a student's final score based on key academic and behavioral factors. It uses synthetic data to simulate a real-world educational dataset and evaluates multiple regression models.

## 📋 Project Overview
The goal is to understand how variables like study habits and attendance influence academic outcomes. The pipeline covers:
- **Data Generation**: Creating a synthetic dataset of 500 students.
- **EDA**: Visualizing correlations and feature distributions.
- **Modeling**: Training and comparing Linear Regression, Decision Trees, and Random Forests.
- **Inference**: A functional prediction system for new inputs.

## 📊 Dataset Features
- `Study_Hours`: Number of hours spent studying (1-10).
- `Attendance`: Percentage of classes attended (60-100%).
- `Previous_Score`: Grades from previous assessments (40-100).
- `Extracurricular`: Binary indicator (0 or 1) for participation in activities.
- `Final_Score`: The target variable (calculated with added Gaussian noise).

## 🚀 Model Performance
Based on the current evaluation, the models achieved the following metrics on the test set:

| Model | MAE | MSE | R2 Score |
| :--- | :--- | :--- | :--- |
| Linear Regression | ~1.68 | ~4.59 | ~0.97 |
| Random Forest | ~2.13 | ~7.66 | ~0.95 |
| Decision Tree | ~2.99 | ~14.22 | ~0.90 |

## 🛠️ Tech Stack
- **Language**: Python
- **Libraries**: Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn
- **Environment**: Google Colab / Jupyter Notebook

## 📝 How to Use
1. Run the notebook to generate the `student_performance.csv` file.
2. Execute the training cells to initialize the models.
3. Use the `predict_student_score` function to estimate scores for new data points.
