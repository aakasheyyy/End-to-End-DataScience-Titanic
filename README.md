COMPANY:CODTECH IT SOLUTIONS

NAME:AAKASH R

INTERN ID:CT04DR985

DOMAIN:DATA SCIENCE

DURATION:4 WEEKS

MENTOR:NEELA SANTHOSH

Automated ETL pipeline in Python using Pandas & Scikit-learn

# End-to-End-DataScience-Titanic
End-to-end data science project predicting Titanic passenger survival using Python, Random Forest, and Flask API deployment.COMPANY:CODTECH IT SOLUTIONS

Project Overview

This project is a complete end-to-end data science workflow predicting the survival of Titanic passengers.
It covers data collection, preprocessing, EDA, model building, evaluation, and deployment as a Flask API.

The project demonstrates real-world skills in machine learning, data visualization, and web deployment.

Key Features

Predict survival using passenger data (Pclass, Sex, Age, Fare, etc.)

Preprocessed and cleaned data for high accuracy

Explored relationships between features using visualizations

Built a Random Forest Classifier achieving 82% accuracy

Deployed model via Flask API for live predictions

Project Steps
1. Data Collection

Dataset: Titanic dataset from DataScienceDojo

Features include: PassengerId, Pclass, Name, Sex, Age, SibSp, Parch, Fare, Embarked

2. Data Preprocessing

Handled missing values (Age → median, Embarked → mode)

Dropped unnecessary columns (Name, Ticket, Cabin, PassengerId)

Encoded categorical variables (Sex, Embarked) to numerical columns

3. Exploratory Data Analysis (EDA)

Visualized survival counts and survival by Sex and Pclass

Plotted distributions of Age and Fare

Correlation heatmap to understand feature importance

4. Model Building

Split dataset into train (80%) and test (20%)

Trained a Random Forest Classifier

Evaluated using accuracy, confusion matrix, and classification report

Results:

Accuracy: 0.82
Confusion Matrix:
[[91 14]
 [18 56]]

5. Model Deployment

Saved the trained model with joblib

Built a Flask API with /predict endpoint

Users can send passenger data as JSON to receive survival prediction

Sample API Request:

POST /predict
{
  "Pclass": 3,
  "Age": 22,
  "SibSp": 1,
  "Parch": 0,
  "Fare": 7.25,
  "Sex_male": 1,
  "Embarked_Q": 0,
  "Embarked_S": 1
}


Response:

{
  "Survived": 0
}

Tools & Libraries

Python 3

Pandas, NumPy

Matplotlib, Seaborn (EDA)

Scikit-learn (Random Forest Classifier)

Flask (API Deployment)

Joblib (Model Saving) 
