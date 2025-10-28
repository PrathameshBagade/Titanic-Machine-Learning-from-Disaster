# 🚢 Titanic: Machine Learning from Disaster

This is my first end-to-end data science project, focused on predicting passenger survival from the 1912 Titanic disaster. The goal is to build a machine learning model that predicts whether a passenger survived (`1`) or did not (`0`) based on features like age, gender, and ticket class.

---

## 📌 1. Project Overview & Problem Statement

- **Problem**: Given a set of passenger attributes, can we build a model to accurately predict if that passenger survived?
- **Task**: Binary classification problem.
- **Dataset**: Sourced from the [Kaggle Titanic competition](https://www.kaggle.com/c/titanic), loaded via URL in the script.

---

## 🔄 2. Project Workflow

The project follows the standard data science lifecycle:

- **Data Loading**: Loaded `titanic.csv` using the Pandas library.
- **Exploratory Data Analysis (EDA)**: Explored patterns and insights using Matplotlib and Seaborn.
- **Data Cleaning & Feature Engineering**:
  - Filled missing `Age` values with the mean.
  - Converted categorical features like `Sex` into numerical format.
- **Model Building**: Applied Logistic Regression — a robust and interpretable model for binary classification.
- **Model Evaluation**:
  - Split data into 80% training and 20% testing.
  - Evaluated using accuracy score and confusion matrix.

---

## 📊 3. Key Findings from EDA

Visualizations revealed several factors influencing survival:

- **Gender**: Female passengers had a significantly higher survival rate than males — supporting the "women and children first" protocol.
- **Ticket Class (`Pclass`)**: 
  - 1st class passengers had the highest survival rate.
  - 3rd class passengers had the lowest — indicating a strong socio-economic influence.
- **Age**: Young children showed a higher chance of survival.

---

## 🤖 4. Model & Results

- **Model Used**: Logistic Regression (scikit-learn)
- **Features Used**: `Pclass`, `Sex`, `Age`, `Fare`
- **Performance**: Achieved ~80% accuracy on the test dataset.

### Confusion Matrix

