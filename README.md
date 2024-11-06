#Fatigue Risk Prediction Model

This project predicts the "fatigue risk" based on health metrics using a Random Forest Classifier. It analyzes daily data over a month, including steps, heart rate, sleep hours, calories consumed, and mood. The model aims to identify fatigue risk for personalized health recommendations, particularly for those at risk of fatigue due to high heart rate and insufficient sleep.

Project Overview
The project generates synthetic data for a 30-day period and builds a binary classification model to predict fatigue risk. Fatigue risk is determined based on a combination of high heart rate (>100 bpm) and insufficient sleep (<6 hours). The model uses Random Forest with hyperparameter tuning to optimize accuracy.

Key Features
Data Generation: Generates a synthetic dataset with daily metrics.
Feature Engineering: Adds a 7-day moving average for steps and one-hot encodes mood.
Binary Target Creation: Sets a binary target variable (fatigue_risk) based on health conditions.
Class Imbalance Handling: Uses upsampling to balance the classes.
Hyperparameter Tuning: Utilizes grid search for optimized model parameters.
Model Persistence: Saves the trained model using pickle for future use.

Technologies Used
Python: Core programming language
NumPy & Pandas: Data manipulation and analysis
Scikit-Learn: Model training and evaluation
GridSearchCV: Hyperparameter tuning
Pickle: Model persistence
