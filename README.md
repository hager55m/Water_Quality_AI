Project Overview
Access to clean, safe drinking water is crucial for health and development. This project focuses on predicting the potability (safety for drinking) of water samples by analyzing their physical and chemical properties. We applied various machine learning models to determine whether the water is safe for consumption or requires further testing.

Objective
The goal is to build a reliable classification model that can predict whether water samples are potable based on their features. We utilize data preprocessing, exploratory data analysis (EDA), feature engineering, and machine learning algorithms to achieve optimal results.

Project Structure
Data Preprocessing

Handling Duplicates: Ensured no duplicate rows in the dataset.
Missing Values: Imputed missing values for pH, Sulfate, and Trihalomethanes using mean and median values.
Outlier Detection and Handling: Identified outliers using box plots and transformed the affected features.
Feature Scaling: Applied MinMaxScaler to features such as Conductivity, Solids, and Hardness to improve model performance.
Correlation Analysis: Created a correlation heatmap to analyze relationships between features.
Class Imbalance

Addressed the imbalance in potable vs. non-potable samples using SMOTE (Synthetic Minority Over-sampling Technique) to ensure balanced model training.
Modeling
Several machine learning models were trained and tuned, including:

K-Nearest Neighbors (KNN): Tuned using GridSearchCV and evaluated with accuracy, precision, recall, and F1-score.
Decision Tree: Optimized using parameters such as min_samples_split and max_depth.
Random Forest: Fine-tuned with n_estimators, min_samples_split, and max_depth to maximize accuracy.
Other Models: Also experimented with Logistic Regression and Support Vector Machine (SVM).
Evaluation

Models were evaluated based on accuracy, precision, recall, F1-score, and confusion matrices.
Cross-validation was used to ensure robust model performance and avoid overfitting.
Best Model: KNN with n_neighbors = 23 emerged as the best-performing model based on cross-validation and overall metrics.
Dataset
The dataset used for the project is publicly available and contains the following features:

pH: pH level of the water (0 to 14).
Hardness: Hardness of the water (mg/L).
Solids: Total dissolved solids in parts per million (ppm).
Chloramines: Concentration of chloramines (ppm).
Sulfate: Sulfate concentration (mg/L).
Conductivity: Electrical conductivity (μS/cm).
Organic Carbon: Organic carbon concentration (ppm).
Trihalomethanes: Trihalomethanes concentration (μg/L).
Turbidity: Water clarity measured in NTU.
Potability: Indicator of whether the water is potable (1 = potable, 0 = non-potable).
