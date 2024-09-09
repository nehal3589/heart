# Heart Disease Prediction using Machine Learning Techniques

## Table of Contents
1. [Introduction](#introduction) 
2. [Exploratory Data Analysis](#exploratory-data-analysis) 
3. [Gaussian Naive Bayes](#gaussian-naive-bayes) 
4. [Logistic Regression](#logistic-regression) 
5. [Linear Discriminant Analysis (LDA)](#linear-discriminant-analysis-lda) 
6. [Quadratic Discriminant Analysis (QDA)](#quadratic-discriminant-analysis-qda)
7. 

## Introduction
The dataset under examination is a classic resource used in medical diagnostics, particularly for predicting heart disease. Originating from databases compiled in 1988, this dataset includes records from Cleveland, Hungary, Switzerland, and Long Beach V. It features 76 attributes, with 14 key attributes commonly used for analysis and prediction.

The goal is to build predictive models and perform statistical analyses to identify patterns and relationships that may indicate heart disease. Various machine learning techniques will be applied, and their effectiveness in classifying patients based on their attributes will be evaluated.

## Exploratory Data Analysis
*Attributes of the dataset:*
- age: Age of the patient (integer)
- sex: Gender (1 = male, 0 = female)
- cp: Chest pain type (categorical, encoded as integers)
- trestbps: Resting blood pressure (integer)
- chol: Serum cholesterol in mg/dl (integer)
- fbs: Fasting blood sugar > 120 mg/dl (1 = true, 0 = false)
- restecg: Resting electrocardiographic results (categorical, encoded as integers)
- thalach: Maximum heart rate achieved (integer)
- exang: Exercise-induced angina (1 = yes, 0 = no)
- oldpeak: ST depression induced by exercise relative to rest (float)
- slope: Slope of the peak exercise ST segment (categorical, encoded as integers)
- ca: Number of major vessels colored by fluoroscopy (integer)
- thal: Thalassemia (categorical, encoded as integers)
- target: Target variable indicating the presence of heart disease (1 = disease, 0 = no disease)

![image](https://github.com/user-attachments/assets/13d3668b-ff73-4fba-91da-83175b2c8794)


The dataset contains 14 columns and 1025 rows.

We used the describe function to obtain an overview of data distribution and basic statistics. Data quality was checked using isnull().sum().

## Gaussian Naive Bayes
The Gaussian Naive Bayes algorithm is used as it is well-suited for continuous features. The dataset is split into training (67%) and testing (33%) sets. The model achieved an accuracy of 85%, with 34 false positives and 15 false negatives.

![image](https://github.com/user-attachments/assets/2d52c70a-a0d8-4bb9-a35f-fcf7b134d291)


## Logistic Regression
Logistic regression was applied to analyze patient data and predict the probability of developing heart disease based on age. After training, the model predicted a high probability of disease for a 46-year-old person.

<img src="https://github.com/user-attachments/assets/50ead4fa-3109-4039-9154-919f3386b6d3" alt="image" style="width:50%; height:auto;"/>


## Linear Discriminant Analysis (LDA)
Linear Discriminant Analysis (LDA) projects data onto a line to maximize class separation and minimize variance. The LDA model achieved an accuracy of 84.18%. It performed well in identifying patients with heart disease (recall: 0.90) and those without (recall: 0.78). The precision was 0.88 for no disease and 0.81 for disease.

![image](https://github.com/user-attachments/assets/828b85c2-50d9-49ff-b682-4a89d2120b82)

## Quadratic Discriminant Analysis (QDA)
Quadratic Discriminant Analysis (QDA) allows for different variances between classes and finds quadratic surfaces to separate them. The QDA model achieved an accuracy of 82.14%. It performed better at identifying patients without heart disease (precision: 0.87) than those with heart disease (precision: 0.78). There were 36 false positives and 19 false negatives.

![image](https://github.com/user-attachments/assets/e8fb8b27-1daa-4b39-a6ce-48a76477ca70)


## Credits

This file was created by:
- Joud Ahmad Al-huthaly (https://github.com/BYXDATA)
- Nehal Hamed Al-zahrani(https://github.com/nehal3589)
