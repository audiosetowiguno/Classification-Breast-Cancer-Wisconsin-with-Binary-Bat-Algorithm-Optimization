# 🧠 Classification Breast Cancer Wisconsin with Binary Bat Algorithm Optimization

## 📍 Introduction
Breast cancer is one of the frequently diagnosed types of cancer in women. It occurs due to the aberrant growth of cells that have lost their normal control mechanisms, leading to abnormal, rapid, and uncontrolled growth. Breast cancer is considered a leading cause of death worldwide, with an estimated 8.2 million deaths. This mortality rate can be reduced by enhancing awareness, prediction, and early diagnosis by medical professionals. Accurate prediction and diagnosis results can ensure that medical interventions are tailored to the patient's condition. Therefore, this project aims to develop a classification model for breast cancer patients using the Logistic Regression, Random Forest, and MLP Classifier methods, coupled with Binary Bat Algorithm for feature selection. 

This project utilizes the Breast Cancer Wisconsin (Diagnostic) dataset obtained from Kaggle ([Datasets Breast Cancer Wisconsin](https://www.kaggle.com/datasets/uciml/breast-cancer-wisconsin-data)). The dataset comprises 568 patients with 32 attributes, where the target variable is 'diagnosis,' containing values of Malignant and Benign. Malignant tumors are cancerous growths characterized by uncontrolled cell growth and the ability to invade surrounding tissues or spread to other parts of the body. Benign tumors are non-cancerous growths characterized by localized and controlled cell growth.

In the previous research by V.Nanda Gopal et all (2021), the correlation function was employed to obtain the best features, resulting in the evaluation performance scores as follows:

| Evaluation | Random Forest | Logistic Regression | MLP Classifier |
| --------------- | --------------- | --------------- |--------------- |
| Precicion | 90%   | 78%   | 98%  |
| Recall  | 94%   | 79%    | 97%   |
| F1-Score   | 92%   | 78%   | 96%   |
| Accuracy    | 95%   | 79%   | 98%   |

## 📍 Objective
In this project, I employ the Binary Bat Algorithm for feature selection to compare its evaluation with the results obtained in the previous research. This enables us to determine the superior feature selection method between the Binary Bat Algorithm and the Correlation Function. 

## 🧪 Data Preprocessing
  - Handling Missing Values
  - Label Encoder (Target)
  - Data Transformation
  - Handling Outlier

## Conclusion After Apply Binary Bat Algorithm for each classification

From the three classifications using Binary Bat Algorithm optimization, 19 best features were obtained with the highest accuracy rate in the MLP Classifier model, achieving a training accuracy of 97.7% and a test accuracy of 99.1%. The selected best features are as follows: [`radius_mean`, `perimeter_mean`, `concave points_mean`, `symmetry_mean`, `fractal_dimension_mean`, `radius_se`, `texture_se`, `perimeter_se`, `smoothness_se`, `concavity_se`, `concave points_se`, `symmetry_se`, `fractal_dimension_se`, `radius_worst`, `texture_worst`, `area_worst`, `smoothness_worst`, `concavity_worst`, `symmetry_worst`].

  - Using Correlation Function
Evaluation table in the study by V. Nanda Gopal et al. (2021) using correlation function.

| Evaluation | Random Forest | Logistic Regression | MLP Classifier |
| --------------- | --------------- | --------------- |--------------- |
| Precicion | 90%   | 78%   | 98%  |
| Recall  | 94%   | 79%    | 97%   |
| F1-Score   | 92%   | 78%   | 96%   |
| Accuracy    | 95%   | 79%   | 98%   |

  - Using Binary Bat Algorithm
Evaluation table using Binary Bat Algorithm Optimization.

| Evaluation | Random Forest | Logistic Regression | MLP Classifier |
| --------------- | --------------- | --------------- |--------------- |
| Precicion | 95%   | 98%   | 98%  |
| Recall  | 95%   | 98%    | 98%   |
| F1-Score   | 95%   | 98%   | 98%   |
| Accuracy    | 95%   | 98%   | 98%   |

In the three classification methods used, there was an improvement in the performance evaluation metrics. In the logistic regression model, there was a significant increase in performance metrics by approximately 20% for each evaluation metric. Similarly, in the Random Forest and MLP methods, there was an improvement in evaluation metrics (Precision, Recall, F1-score, and accuracy).

---
Thus, the best classification method used to classify classes in the Wisconsin Breast Cancer dataset is the MLP Classifier, and feature selection using Binary Bat Algorithm is better than to correlation function.



