## Introduction
This project aims to predict equipment failures using machine learning techniques. The goal is to help in preventive maintenance by identifying potential failures before they occur, thereby reducing downtime and maintenance costs.

## Dataset
The dataset used in this project contains various metrics collected from different devices. Each entry in the dataset represents a snapshot of the device's state at a given time, including whether a failure occurred.

## Data Preprocessing
### Steps Involved:
- Data Cleaning: Remove redundant and irrelevant columns.
- Data Transformation: Convert categorical variables into dummy variables and handle skewness in numerical variables using log transformation.
- Feature Scaling: Apply standardization to numerical features.
- Feature Selection: Select important features using feature importance scores from a tree-based model.
## Model Training
The following models were trained on the preprocessed data:

- Logistic Regression
- Random Forest Classifier
- XGBoost Classifier
### Train-Test Split
The data was split into training and testing sets using an 75-25 split.

## Hyperparameter Tuning
GridSearchCV was used to perform hyperparameter tuning for the Random Forest and XGBoost models to find the best set of parameters.

## Evaluation
The performance of the models was evaluated using the following metrics:

- Precision
- Recall
- F1-Score
- ROC-AUC
ROC curves were plotted to visualize the performance of each model.

## Conclusion
The tuned models were able to effectively predict equipment failures, with the XGBoost model showing the best performance. By identifying potential failures early, this project can help in scheduling timely maintenance and reducing downtime.
