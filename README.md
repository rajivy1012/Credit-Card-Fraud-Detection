Dataset Google drive link : https://drive.google.com/drive/folders/1b4aL0Q8tHh3Hyzzv5D5zENfAoBbGMBQi?usp=sharing
-----


Methodology:
--------

This study investigates the effectiveness of credit card fraud detection methods using a dataset obtained from Kaggle. The objective is to examine various features and their role in identifying fraudulent transactions. The methodology follows a systematic process that includes data preprocessing, exploratory data analysis (EDA), feature engineering, modeling, and performance evaluation.

Data Collection and Preprocessing: The dataset consists of transactional details, including transaction amount, location, demographics, and categorical variables such as merchant and transaction category. The data is initially loaded into a Pandas DataFrame, and irrelevant columns like Unix time and merchant details are discarded.

Exploratory Data Analysis (EDA): EDA is conducted to gain insights into the distribution of data, detect patterns, and understand the relationship between features and the target variable (fraud or non-fraud). Visualizations like pie charts, histograms, and heatmaps are utilized to analyze the distribution of categorical variables, transaction amounts, and correlations between features.

Distribution of Gender With Fraud:
----
![image](https://github.com/rajivy1012/Credit-Card-Fraud-Detection/assets/157632817/cd33b186-2cea-4423-b2a0-60845defeb68)

Age Distribution : 
![image](https://github.com/rajivy1012/Credit-Card-Fraud-Detection/assets/157632817/df230a8b-677a-45a5-8545-706e7f243043)

Fraud Transaction Timing:
![image](https://github.com/rajivy1012/Credit-Card-Fraud-Detection/assets/157632817/b1c7ae5f-8fc7-46f8-93a0-c1d4a72a6820)

 
Feature Engineering :  Categorical variables are encoded using methods like Weight of Evidence (WOE) encoding to convert them into numerical representations. Additionally, age is computed from the date of birth, and the transaction hour is extracted from the timestamp to enhance the predictive capability of the model.


Modeling:
----
The primary model chosen is the Random Forest Classifier, known for its ability to handle imbalanced datasets and produce interpretable results. The dataset is split into training and testing sets, and the model is trained using the training data. Model performance is evaluated using metrics such as accuracy, precision, recall, and F1-score.

Performance Evaluation:
-----
The performance of the trained model is assessed on the test dataset using classification metrics and visualizations like confusion matrices and ROC curves. The classification report provides insights into the model's precision, recall, and F1-score for both fraudulent and non-fraudulent transactions.
![image](https://github.com/rajivy1012/Credit-Card-Fraud-Detection/assets/157632817/d78c98f1-d5e6-4852-99bb-81227e32457e)

Results:
----
The Random Forest Classifier achieves a high accuracy of 99.89% and a precision score of 96.27% in identifying fraudulent transactions. The analysis of the ROC curve indicates a high Area Under the Curve (AUC) score, confirming the effectiveness of the model in distinguishing between fraud and non-fraud cases.
![image](https://github.com/rajivy1012/Credit-Card-Fraud-Detection/assets/157632817/1683f0fa-fcab-4409-b6ec-ca61e3b7b8f6)

 
