Project Overview
Clean, safe drinking water is super important for health and development! 🌍💧 This project is all about predicting if water samples are potable (safe to drink) or not, using various physical and chemical properties. We’re diving into different machine learning models to figure out whether your water is ready for a sip or needs some more testing. 🧪📊

Objective
We want to build a trusty classification model that can tell if water samples are safe to drink based on their features. We’ll use data preprocessing, exploratory data analysis (EDA), feature engineering, and machine learning algorithms to get the best results. 🏆💡

Project Structure
1. Data Preprocessing 🛠️
Handling Duplicates: Double-checked and made sure there are no duplicate rows.
Missing Values: Filled in missing values for ph, Sulfate, and Trihalomethanes with mean and median values.
Outlier Detection and Handling: Found outliers, visualized them with box plots, and transformed those tricky features.
Feature Scaling: Scaled features like Conductivity, Solids, and Hardness using MinMaxScaler to help the models work better.
Correlation Analysis: Made a cool correlation heatmap to see how features relate to each other.
2. Class Imbalance ⚖️
Our dataset had more non-potable samples, so we used SMOTE (Synthetic Minority Over-sampling Technique) to balance things out.
3. Modeling 🤖
We tried out and compared several machine learning models:

K-Nearest Neighbors (KNN): Tuned with GridSearchCV and checked accuracy, precision, recall, and F1-score.
Decision Tree: Adjusted parameters like min_samples_split and max_depth for better results.
Random Forest: Fine-tuned n_estimators, min_samples_split, and max_depth to boost accuracy.
Other Models: Also gave Logistic Regression and SVM (Support Vector Machine) a spin.
4. Evaluation 📈
We checked out models based on accuracy, precision, recall, F1-score, and confusion matrices.
Used cross-validation to make sure our models were solid and not overfitting.
Best Model: KNN with n_neighbors = 23 was the champ based on cross-validation and overall performance.
Dataset
The dataset is publicly available and includes:

pH: pH level of the water (0 to 14).
Hardness: How hard the water is, measured in mg/L.
Solids: Total dissolved solids in ppm.
Chloramines: Amount of chloramines in ppm.
Sulfate: Amount of sulfates in mg/L.
Conductivity: Electrical conductivity in μS/cm.
Organic Carbon: Amount of organic carbon in ppm.
Trihalomethanes: Amount of Trihalomethanes in μg/L.
Turbidity: How clear the water is, measured in NTU.
Potability: Whether the water is potable (1) or not (0).
