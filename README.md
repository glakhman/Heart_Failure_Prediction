# Project 2: Heart Failure Prediction

## Introduction to the Problem
Cardiovascular diseases (CVDs) are the number one cause of death globally, taking an estimated 17.9 million lives each year, which accounts for 31% of all deaths worldwide. Four out of five cardiovascular disease deaths are due to heart attacks and strokes, and one-third of these deaths occur prematurely in people under 70 years of age.  

Heart failure is a common event caused by CVDs and this dataset contains 11 features that can be used to predict a possible heart disease. People with cardiovascular disease or who are at high cardiovascular risk (due to the presence of one or more risk factors such as hypertension, diabetes, hyperlipidaemia, or already established disease) need early detection and management in which a machine learning model could be of great help.

**Key Questions**
- What are some common features of heart failure?  
- How can we use different attribute information for early detection?  
- What properties are most present in someone with heart failure?  
- What is the best classification algorithm for this dataset?  

---

## Data Introduction
The dataset used was found on Kaggle and is called **“Heart Failure Prediction Dataset - 11 clinical features for predicting heart disease events”** by [fedesoriano](https://www.kaggle.com/fedesoriano/heart-failure-prediction).  

The purpose of this dataset is to apply classification algorithms to multiple valued attributes in order to identify and predict heart disease in a person based on medical features.  

It contains examples of different leading factors in cardiovascular disease and uses features such as age, blood pressure, cholesterol, exercise, and blood sugar to help predict heart failure.

---

## Pre-processing the Data
My goal for pre-processing the dataset was to ensure consistency, accuracy, and completeness.  

Steps included:
- Inspecting the dataset using **Pandas** and **NumPy**.  
- Identifying categorical features (e.g., fasting blood sugar is categorical: `1 = high`, `0 = low`).  
- Handling correlations (e.g., `ST_Slope_Flat` and `ST_Slope_Up` were highly negatively correlated at -0.92, so one was dropped).  
- Transposing data types for consistency.  
- Filtering out outliers.  
- Visualizing distributions with **boxplots**.  

---

## Data Understanding / Visualization
- **Age vs Heart Disease** → Older people are more likely to have heart disease.  
- **Resting Blood Pressure** → Higher levels increase the probability of heart disease.  
- **Chest Pain Types** → Those with exercise-induced angina are more prone to cardiovascular disease.  
- **Gender** → Men are at higher probability of having heart disease.  
- **Scatter Plots** → Useful for exploring relationships between categorical and numerical features.  

---

## Modeling / Evaluation
The task was to predict whether a person has cardiovascular disease based on health features.  

**Algorithms Used**
- Logistic Regression  
- Support Vector Machine (SVM)  

**Why Logistic Regression?**
- Helps understand the relationship between dependent and independent variables.  
- Lower false negatives (important in medical contexts).  

**Why SVM?**
- Effective at drawing decision boundaries.  
- Performed well, but predicted more false positives compared to Logistic Regression.  

**Comparison**
- Logistic Regression performed better overall due to lower false negatives.  
- K-Nearest Neighbors was considered but discarded due to weaker performance compared to Logistic Regression.  

---

## Results
- **Logistic Regression** → Best overall model with fewer false negatives.  
- **SVM** → Still effective but less optimal due to higher false positives.  

---

## Storytelling
After visualizing a large portion of the data, I gained valuable understanding of the common attributes linked to cardiovascular disease.  

This project helped me:
- Identify key attributes related to heart disease.  
- Practice dataset preprocessing (cleaning, correlation handling, and outlier removal).  
- Use data visualization to interpret medical features.  
- Compare machine learning models for predictive performance.  

One of the most challenging parts was formatting and executing dataset transformations in a clear way. Overall, I learned a great deal about collecting data, preprocessing, relationships in data, and model evaluation.

---

## References / Code
- Dataset: [Kaggle - Heart Failure Prediction](https://www.kaggle.com/fedesoriano/heart-failure-prediction)  

