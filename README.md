HEART DISEASE PREDICTION

The notebook is based on predicting heart disease using various machine learning models. Here's a breakdown of the project components:

### Problem Statement:
The goal of this project is to predict the likelihood of heart disease in patients based on various medical features such as age, blood pressure, cholesterol levels, and other diagnostic measurements. The model aims to aid in early detection and decision-making for healthcare professionals.

### Dataset:
The dataset contains multiple medical features that could be indicators of heart disease, including:
- Age
- Sex
- Chest pain type
- Resting blood pressure
- Serum cholesterol
- Fasting blood sugar
- Resting electrocardiographic results
- Maximum heart rate achieved
- Exercise-induced angina
- ST depression induced by exercise relative to rest
- Slope of the peak exercise ST segment
- Number of major vessels colored by fluoroscopy
- Thalassemia status (thal)

The target variable is whether the patient has heart disease or not (binary classification).

### Data Preprocessing Techniques:
The following data preprocessing techniques were used to prepare the dataset for model training:
1. **Handling Missing Data**: Missing values were handled by imputing or removing incomplete records.
2. **Encoding Categorical Variables**: Categorical features like sex and chest pain type were encoded into numerical values for model compatibility.
3. **Scaling Features**: Continuous variables such as blood pressure and cholesterol levels were scaled to ensure that no feature dominates the model training due to its magnitude.
4. **Train-Test Split**: The dataset was split into training and testing sets to evaluate model performance.

### Model Selection Table:

| Model               | Training Accuracy (%) | Testing Accuracy (%) |
|---------------------|-----------------------|----------------------|
| Logistic Regression | 88.68                 | 84.62                |
| KNearest Neighbour  | 85.38                 | 82.42                |
| Decision Tree       | 100.00                | 76.92                |

### Finalized Model:
The **Logistic Regression** model is the most balanced in terms of accuracy, showing high performance on both the training and testing datasets. It is less prone to overfitting compared to the Decision Tree model and offers better testing accuracy than KNearest Neighbour. Therefore, **Logistic Regression** is selected as the final model.
