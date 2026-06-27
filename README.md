# Heart Disease Prediction

## Project Overview
This repository contains a Machine Learning project to predict the likelihood of a patient developing heart disease based on various medical attributes. Early detection of cardiovascular diseases can significantly improve patient outcomes, and this project serves as a diagnostic support tool using predictive modeling.

## Dataset
The project utilizes a heart disease dataset (`heart.csv`) containing 14 medical features for 1025 patient records initially. After data cleaning and duplicate removal, the dataset contains 302 unique patient records.

**Key Features:**
* `age`: Age of the patient
* `sex`: Gender of the patient
* `cp`: Chest pain type
* `trestbps`: Resting blood pressure (in mm Hg)
* `chol`: Serum cholesterol in mg/dl
* `fbs`: Fasting blood sugar
* `restecg`: Resting electrocardiographic results
* `thalach`: Maximum heart rate achieved
* `exang`: Exercise-induced angina
* `oldpeak`: ST depression induced by exercise relative to rest
* `slope`: The slope of the peak exercise ST segment
* `ca`: Number of major vessels
* `thal`: Presence of fixed or reversible defects
* `target`: Presence of heart disease (1 = yes; 0 = no)

## Workflow & Exploratory Data Analysis (EDA)
* **Data Cleaning:** Identified and removed 723 duplicate records. Rounded the `oldpeak` feature to integer values. Verified that the dataset contains zero null values.
* **Statistical Summary:** Analyzed standard deviations, means, and boundary values across all 14 parameters.
* **Correlation Analysis:** Plotted a Seaborn correlation heatmap to visualize the linear relationships between physiological features and the target variable.

## Machine Learning Models
The project imports and sets up comparisons for distinct machine learning algorithms:
* **Linear Regression / Logistic Regression:** Analyzes continuous probability risk for binary classification. 
* **Random Forest Classifier:** An ensemble learning method using multiple decision trees to improve predictive accuracy.
* **K-Nearest Neighbors (KNN):** A distance-based algorithm classifying patients based on the proximity of their attributes.

## Results
All models were evaluated based on their accuracy in predicting the `target` variable. 
* **Top Performing Model:** The **K-Nearest Neighbors (KNN)** model achieved the highest overall accuracy, demonstrating its strong capability in mapping similarities between patient health indicators.

## Requirements
* `pandas`
* `numpy`
* `matplotlib`
* `seaborn`
* `scikit-learn`


