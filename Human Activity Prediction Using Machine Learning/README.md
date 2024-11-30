# Human Activity Prediction Using Machine Learning

This project uses wearable sensor data to predict human activities based on machine learning techniques.

## Dataset

Human Activity Recognition database built from the recordings of 30 subjects performing activities of daily living (ADL) while carrying a waist-mounted smartphone with embedded inertial sensors.

### Citation
Reyes-Ortiz, J., Anguita, D., Ghio, A., Oneto, L., & Parra, X. (2013). Human Activity Recognition Using Smartphones [Dataset]. UCI Machine Learning Repository. https://doi.org/10.24432/C54S4K.

## Objective
The goal of this project is to classify and predict human activities (e.g., walking, sitting, standing) using wearable sensor data and machine learning techniques.

## Approach

The goal of this project was to classify human activity based on sensor data from wearable devices. 
1. **Data Preprocessing**: 
   - Loaded and explored the dataset.
   - Handled missing values (if any) and cleaned the data.
2. **Feature Engineering**: 
   - Selected relevant features for modeling.
   - Applied techniques like outlier detection using IQR and PCA for dimensionality reduction.
3. **Model Building**:
   - Tried different models like Random Forest, Logistic Regression, and Support Vector Machine.
4. **Model Evaluation**: 
   - Evaluated the models based on metrics like accuracy, precision, and recall.

## Techniques Used

### 1. Outlier Detection: IQR * 1.5 Method
Outliers were detected using the Interquartile Range (IQR) method, with a threshold of 1.5 times the IQR. Outliers were replaced with the median value of their respective features.

### 2. Normality Testing: Kolmogorov-Smirnov Test
The Kolmogorov-Smirnov test was used to check for normality. Since many features were non-normally distributed, non-parametric methods like IQR were preferred over z-scores.

### 3. PCA (Principal Component Analysis)
PCA was applied to reduce dimensionality, retaining 95% of the variance. This was done to remove multicollinearity and reduce computational costs for subsequent modeling.

### 4. Classification Models
Three classification models were used for predicting human activity:
- **Random Forest**: An ensemble model for robust predictions.
- **Logistic Regression**: A simple but effective model.
- **SVM**: With an RBF kernel for capturing complex decision boundaries.

## Results
- The Support Vector Machine (SVM) classifier achieved the best accuracy of 95%.
- Dimensionality reduction using PCA reduced the features from 561 to 100 while retaining ~95% of the variance.
- The models successfully classified human activities like walking, sitting, and standing with high precision and recall.
