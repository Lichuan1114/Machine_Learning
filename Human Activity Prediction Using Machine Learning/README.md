# Human Activity Prediction Using Machine Learning

This project uses wearable sensor data to predict human activities based on machine learning techniques.

## Dataset

Human Activity Recognition database built from the recordings of 30 subjects performing activities of daily living (ADL) while carrying a waist-mounted smartphone with embedded inertial sensors.

### Citation
Reyes-Ortiz, J., Anguita, D., Ghio, A., Oneto, L., & Parra, X. (2013). Human Activity Recognition Using Smartphones [Dataset]. UCI Machine Learning Repository. https://doi.org/10.24432/C54S4K.

## Objective
The goal of this project is to classify and predict human activities (e.g., walking, sitting, standing) using wearable sensor data and machine learning techniques.

## Approach
- Performed Exploratory Data Analysis (EDA) to understand the data and its distribution.
- Preprocessed the data by addressing missing values and outliers.
- Reduced dimensionality using Principal Component Analysis (PCA) to eliminate redundancy in features.
- Trained and evaluated three classifiers: Random Forest, Logistic Regression, and Support Vector Machines (SVM).

## Results
- The Support Vector Machine (SVM) classifier achieved the best accuracy of 95%.
- Dimensionality reduction using PCA reduced the features from 561 to 100 while retaining ~95% of the variance.
- The models successfully classified human activities like walking, sitting, and standing with high precision and recall.
