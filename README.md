# Student-Performance-Predictor
This project implements a simple machine learning pipeline using a Random Forest Classifier to predict whether a student will pass an examination based on key academic factors.
The script includes functionalities for generating synthetic training data, training the model, saving the trained model and its performance summary, and providing an interactive command-line interface for making predictions and analyzing feature importance.
The model is trained on simulated data using features such as study hours, attendance rate, assignments completed, and previous scores.

# Features
Synthetic Data Generation: Automatically creates a CSV file (students.csv) with simulated student data for training.
-Random Forest Training: Trains an \text{scikit-learn} RandomForestClassifier for binary classification (Pass/Fail).
-Model Persistence: Saves the trained model (rf_model.pkl) and a performance summary (model_summary.json) for later use.
-Interactive Menu: Provides a simple command-line interface to:
1.Retrain the model.
2.Predict the Pass/Fail outcome for a new student with probability scores.
3.View the ranking of features by their importance in the prediction (Feature Importance).
-Performance Metrics: Calculates and saves the model's accuracy and a detailed classification report.

# Installation
To set up and run this project locally, you need Python and the following packages.
Prerequisites
Python 3.x
Dependencies
The required libraries are:
numpy
pandas
scikit-learn
joblib
You can install all dependencies using pip:
pip install numpy pandas scikit-learn joblib

# Usage
Run the main Python script from your terminal. If a model doesn't exist, it will automatically train one.
python your_script_name.py

# Example Prediction
Choice: 2
Study hours: 8.5
Attendance %: 92.0
Assignments done: 9
Previous score: 85.5

Prediction: pass
Pass prob: 0.95
Fail prob: 0.05

# Project Structure
The project will generate the following files upon initial run:
1.students.csv: The synthetic dataset used for training.
2.rf_model.pkl: The serialized Random Forest model object (using \text{joblib}).
3.model_summary.json: A JSON file containing the training date, accuracy, dataset size, and classification report.
