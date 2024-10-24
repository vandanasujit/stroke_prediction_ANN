# Stroke Prediction using Artificial Neural Networks (ANN)
###Project Overview
This project focuses on predicting the likelihood of a stroke in individuals using various medical and lifestyle features. The dataset contains several features like age, gender, hypertension, heart disease, BMI, glucose levels, and more. An Artificial Neural Network (ANN) is utilized to make predictions, and the model's performance is evaluated to determine its effectiveness.

###Dataset
The dataset consists of 5,110 records with the following features:
id: Unique identifier for each record
gender: Gender of the individual
age: Age of the individual
hypertension: Indicates if the individual has hypertension (0 = No, 1 = Yes)
heart_disease: Indicates if the individual has heart disease (0 = No, 1 = Yes)
ever_married: Marital status of the individual
work_type: Type of employment of the individual
Residence_type: Urban or rural residence
avg_glucose_level: Average glucose level in the blood
BMI: Body Mass Index
smoking_status: Smoking habits of the individual
stroke: Target variable indicating if the individual has had a stroke (0 = No, 1 = Yes)

###Objective
The goal of this project is to predict the occurrence of stroke using machine learning, specifically Artificial Neural Networks (ANN), based on the features provided in the dataset. Since the dataset comes from the healthcare domain, achieving high recall is particularly important to minimize false negatives.

###Model
The model implemented is an Artificial Neural Network (ANN) with the following configuration:
Hidden Layers: Three layers with 100, 50, and 30 neurons respectively
Activation Function: ReLU
Optimizer: Adam
Evaluation Metrics: Accuracy, Precision, Recall, F1-Score, and AUC-ROC.

###Methodology
Data Preprocessing: Handled missing values, normalized numerical data, and encoded categorical variables.
Model Building: Implemented the ANN model using the MLPClassifier from sklearn.
Evaluation: Evaluated the model performance with various metrics, with a focus on the recall rate for the minority class (stroke cases).
Results
The model is evaluated on various metrics, and the performance is compared before and after applying techniques such as oversampling (SMOTE) to handle class imbalance.
