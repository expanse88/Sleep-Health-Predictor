# 🛌 Sleep Health Predictor 🧠

## 🔍 Overview
This project builds a machine learning model to predict sleep disorders (Insomnia, Sleep Apnea, or None) based on a person's health and lifestyle metrics like sleep duration, physical activity, stress level, and more.

It is aimed at exploring how behavioral and physiological data can help assess sleep health — a key factor in overall well-being.

## 📂 Dataset
Source: Kaggle - Sleep Health and Lifestyle Dataset

Size: 374 records, 13 columns

Target Variable: Sleep Disorder (None, Insomnia, Sleep Apnea)

## 🧹 Features Used
Feature	Type
Age	Numerical
Gender	Categorical
Occupation	Categorical
Sleep Duration	Numerical
Quality of Sleep	Numerical
Physical Activity Level	Numerical
Stress Level	Numerical
BMI Category	Categorical
Blood Pressure	Categorical
Heart Rate	Numerical
Daily Steps	Numerical

## 🧠 Model Workflow
Data Cleaning:

Dropped irrelevant columns (e.g., Person ID)

Checked and handled missing values

Encoding:

One-hot encoding for categorical variables

Label encoding for the target variable

EDA:

Explored class distributions and feature relationships

Visualized trends using seaborn & matplotlib

Model Training:

Used Random Forest Classifier

Data split: 80% training, 20% testing

Evaluation:

Accuracy: 86%

F1-Score (weighted): 0.86

## 📈 Model Performance
Metric	Score
Accuracy	86%
Precision	87% (weighted)
Recall	86% (weighted)
F1-Score	86% (weighted)

Class 2 (None) had the highest F1-score, while Class 1 (Insomnia) had lower recall — highlighting potential for further improvement.

## 🧪 Tech Stack
Python (Pandas, NumPy)

Scikit-learn

Seaborn & Matplotlib

Jupyter Notebook

## 💡 Future Improvements
Try other models like XGBoost or LightGBM

Improve recall for Insomnia class with SMOTE or class weighting

Build a Streamlit web app for interactive predictions

Deploy on Hugging Face Spaces or AWS

