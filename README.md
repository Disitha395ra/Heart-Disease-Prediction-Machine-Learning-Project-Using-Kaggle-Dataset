# Heart Disease Prediction | Machine Learning Project

![Heart Disease](https://upload.wikimedia.org/wikipedia/commons/thumb/6/6f/Heart_anterior_exterior_view.png/320px-Heart_anterior_exterior_view.png)

## Overview
This project predicts the **presence of heart disease** using machine learning algorithms.  
The dataset is sourced from [Kaggle](https://www.kaggle.com/) and contains medical features of patients. The goal is to predict whether a patient has heart disease or not.

---

## Dataset
The dataset includes patient information such as:

- Age
- Sex
- Chest Pain Type
- Resting Blood Pressure
- Cholesterol
- Fasting Blood Sugar
- Resting ECG
- Maximum Heart Rate
- Exercise Induced Angina
- ST Depression
- Slope of ST Segment
- Number of Major Vessels
- Thalassemia  
- Target (Heart Disease: 0 = No, 1 = Yes)

---

## Machine Learning Models Used

The following models were implemented and tested:

1. **Logistic Regression**  
2. **K-Nearest Neighbors (KNN)**  
3. **Support Vector Classifier (SVC)**  
4. **Decision Tree Classifier**  
5. **Random Forest Classifier**  
6. **XGBoost Classifier**

Each model was trained on the dataset, and predictions were made on the test set.

---

## Accuracy Comparison

The models were evaluated using **accuracy score**, and the results were visualized in a single plot:

```python
# Example code for plotting accuracy
import matplotlib.pyplot as plt

models = ['Logistic Regression', 'KNN', 'SVC', 'Decision Tree', 'Random Forest', 'XGBoost']
accuracy = [accuracy_logistic, accuracy_knn, accuracy_svc, accuracy_tree, accuracy_random, accuracy_xg]

plt.figure(figsize=(10,6))
plt.bar("Logistic regression",Logistic_acc)
plt.ylabel('Accuracy')
plt.title('Comparison of Machine Learning Models for Heart Disease Prediction')
plt.ylim([0,1])
plt.show()
```
Heart-Disease-Prediction/
│
├─ data/                 # Dataset CSV files
├─ notebooks/            # Jupyter notebooks with code
├─ images/               # Accuracy plots, charts
├─ README.md             # Project overview (this file)
└─ requirements.txt      # Required Python libraries

### Model Accuracy Comparison
![Accuracy Plot](images/accuracy_plot.png)
