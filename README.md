# Glassdoor Salary Prediction using Machine Learning

## Project Overview

This project predicts employee salaries using Machine Learning based on company and job-related features from the Glassdoor Jobs dataset. The complete ML pipeline includes data preprocessing, exploratory data analysis (EDA), feature engineering, model training, evaluation, hyperparameter tuning, feature importance analysis, and model deployment.

---

## Problem Statement

Develop a machine learning model that predicts the annual salary of a job candidate using features such as company rating, company age, and technical skills.

---

## Dataset

- Dataset: Glassdoor Jobs Dataset
- File: `glassdoor_jobs.csv`

### Features Used

- Rating
- Company Age
- Python Skill
- SQL Skill
- Excel Skill
- Spark Skill

### Target Variable

- Average Salary (USD per year)

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- XGBoost
- Pickle
- Google Colab

---

## Machine Learning Pipeline

1. Data Loading
2. Data Cleaning
3. Exploratory Data Analysis (EDA)
4. Feature Engineering
5. Train-Test Split
6. Model Training
7. Model Evaluation
8. Hyperparameter Tuning
9. Feature Importance Analysis
10. Model Saving
11. Prediction on Unseen Data

---

## Machine Learning Models

### Model 1
- Linear Regression

### Model 2
- Decision Tree Regressor

### Model 3 (Final Model)
- XGBoost Regressor

---

## Evaluation Metrics

The models were evaluated using:

- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- R² Score

---

## Feature Importance

Feature importance analysis using XGBoost showed that:

- Python Skill was the most important feature.
- Company Age and SQL Skill had a strong impact on salary prediction.
- Rating and Excel Skill had moderate importance.
- Spark Skill contributed the least among the selected features.

---

## Final Model

The XGBoost Regressor was selected as the final model because it achieved the best predictive performance and provided reliable feature importance for model explainability.

---

## Model Deployment

The trained model was saved using Pickle.

```python
pickle.dump(model, open("salary_prediction_model.pkl", "wb"))
```

The saved model was successfully loaded and used to predict salaries for unseen data.

---

## Results

Example Prediction:

**Predicted Salary:** **$125,994.64 per year**

---

## Project Structure

```
Glassdoor-Salary-Prediction/
│
├── FINAL_project_1_glassdoor_ML_Submission1.ipynb
├── glassdoor_jobs.csv
├── salary_prediction_model.pkl
├── requirements.txt
└── README.md
```

---

## How to Run

1. Clone the repository.
2. Install the required libraries.

```
pip install -r requirements.txt
```

3. Open the notebook in Google Colab or Jupyter Notebook.
4. Run all cells from top to bottom.
5. The trained model will predict salaries and save the model as a `.pkl` file.

---

## Conclusion

A complete machine learning salary prediction pipeline was developed using the Glassdoor Jobs dataset. Multiple regression models were trained and evaluated, and the XGBoost Regressor was selected as the final model based on its predictive performance and feature importance analysis. The trained model successfully predicts annual salaries and can be extended for real-world salary estimation and recruitment analytics.

---

## Author

**Maanaav Trivedi**

Computer Science Engineering Student
