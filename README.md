# Heart Attack Prediction 🩺🫀📶
## Introduction
Heart diseases are one of the leading causes of death worldwide. This project focuses on predicting the likelihood of a heart attack based on various health parameters, such as age, cholesterol levels, blood pressure, and other clinical features. Accurate predictions can help in early diagnosis and prevention, reducing healthcare costs and saving lives.

The objective of this analysis is to build a machine learning model to predict heart attacks based on patient data and optimize the accuracy of predictions.
## Dataset
The dataset used contains 303 observations and 14 features, all related to patient health. The target variable is output, which indicates whether the patient is likely to experience a heart attack (1 = more likely, 0 = less likely).

### Key Attributes:
- age: Age of the patient
- sex: Gender (1 = male, 0 = female)
- cp: Chest pain type (categorical)
- trtbps: Resting blood pressure
- chol: Serum cholesterol
- fbs: Fasting blood sugar (binary)
- restecg: Resting electrocardiographic results (categorical)
- thalachh: Maximum heart rate
- exng: Exercise-induced angina (1 = yes, 0 = no)
- oldpeak: ST depression value
- slp: Slope of the ST segment
- caa: Number of vessels colored by fluoroscopy
- thall: Thalassemia (categorical)
- output: Target variable (1 = high risk of heart attack, 0 = low risk)
## Data Analysis
### Data Loading and Exploration
The dataset was loaded using the pandas library. Initial steps included:

- Viewing the first few rows to understand the structure of the dataset.
- Checking dimensions: The dataset contains 303 rows and 14 columns.
- Data summary: Basic descriptive statistics were computed to understand the range, mean, and spread of the data.
### Visualizations
Visual analysis using matplotlib and seaborn was conducted to better understand the distribution of variables and correlations. Key insights include:

- Age Distribution: The age of patients ranges from 29 to 77 years, with a higher incidence of heart attacks in older age groups.
- Cholesterol Levels: Higher cholesterol levels appear to correlate with an increased risk of heart attacks.
- Chest Pain Type: Different types of chest pain are significant indicators, with certain types showing a stronger relationship with heart attack likelihood.
## Data Preprocessing
### Handling Missing Data
- The dataset did not contain significant missing data, so imputation was not required. However, data types and outliers were reviewed to ensure consistency.

### Feature Scaling
- Numerical features such as age, cholesterol levels, and blood pressure were normalized to ensure that machine learning algorithms perform optimally.

### One-Hot Encoding
- Categorical features, such as chest pain type (cp) and resting electrocardiogram results (restecg), were encoded using one-hot encoding to make them suitable for machine learning models.
## Model Building
### Model Selection
Several machine learning models were applied to the dataset to predict the likelihood of heart attacks. These included:

- Logistic Regression: Used for binary classification.
- Random Forest Classifier: A tree-based ensemble method for improving prediction accuracy.
- K-Nearest Neighbors (KNN): A simple, distance-based classifier.
- Support Vector Machines (SVM): For finding the optimal hyperplane to separate classes.
### Model Evaluation
Models were evaluated using metrics such as:

- Accuracy: The percentage of correct predictions.
- Precision: The proportion of positive identifications that were actually correct.
- Recall: The proportion of actual positives identified correctly.
- F1-Score: A balance between precision and recall.
### Results:
- Logistic Regression: 88.52% accuracy
- Random Forest: 85.24% accuracy
- KNN: 83.60% accuracy
- SVM: 91.80% accuracy
The Support Vector Machine model performed the best with a 91.80% accuracy, making it the most suitable for this problem.
## Conclusion
### Key Insights
- Older age, higher cholesterol levels, and specific types of chest pain were the most significant indicators of heart attack risk.
- The Support Vector Machine provided the most accurate predictions, with 91.80% accuracy, making it a reliable model for further analysis or deployment in healthcare settings.
- Early prediction of heart attacks can lead to more timely interventions, potentially saving lives and reducing healthcare costs.
- By utilizing this model, healthcare providers can make informed decisions and allocate resources more effectively.
