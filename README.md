# Referral-Advice
A data mining approach to predicting referral advice for patients suffering from lower back pain
In this project, we have investigated the automation of referral advice for patients with lower back pain based on patient input to a questionnaire. As part of this project, we aimed to reduce the set of questions used to effectively determine the referral advice. We develop, evaluate and interpret five different machine learning models, with our random forest classifier predicting referral advice with an accuracy of over 70 percent. During our research, we use advanced techniques for data pre-processing as well as feature analysis and dimensionality reduction techniques to overcome problems prevalent in healthcare data. The final selection of features reduced the questionnaire from 36 to 7 features.

## The Data set
The dataset consists of 1546 cases of lower back pain provided by the Groningen Spine Center (GSC), containing patient-reported answers to questionnaires, and their respective treatment advice. There were 36 columns which consisted of feature types ranging from numerical, categorical, binary, and ranged scales of 1-10, and an output column containing the suggested treatment type, which contained 5 output classes: 1-Advice, 2-Rehabilitation, 3-Surgery, 4-Injection/Medication, 5-Combination of 1-4.
## Challenges provided by the dataset
1. The dataset contains a significant amount of missing data, we addressed this by using a combination of deletion and statistical imputation.
2. The dataset is imbalanced, with several classes severely underrepresented. We adressed this by utilizing the synthetic minority oversampling technique (SMOTE)
3. The dataset is highly dimensional with 30 input features left after initial pre-processing. We use a combination of feature analysis and dimensionality reduction techniques: Namely Principle Component Analysis (PCA), Recursive Feature Elimination (RFE) and univariate feature filters. In addition we obtained feature importnance from our random forest classifier.

## Jupyter Notebook
The code is written in python and can be accessed from the Jupyter notebook. You can also open the notebook directly using Colab. 
You can find the complete machine learning pipeline build for this project in this notebook, structured into the following section;
- Data Preprocessing:
  - data investigation
  - handling missing values using combination of deletion and imputation approach)
  - Experimen results for deletion only approach
  - SMOTE utlization
  - standard data prepation steps such as scaling and encoding
- Feature analysis
  - PCA & experimentation with Random forest classification
  - RFE & experimentation wih Random forest, XGBoost classification
  - Univariate feature filters & experimentation with Random forest classification
  - Random forest feature importance & experimentation with XGBoost & Decision Tree classification
- ML Model building, evaluation and comparisom on 5-class, 4-class and binary classification (respectively with and without oversampling) using 5 ML models
  - Random forest
  - Suport vektor machine
  - XGBoost
  - Decision Tree
  - Logistic regression
  & 10-fold cross validation
  
  To review this notebook, you can simply open the file inside your browser.


