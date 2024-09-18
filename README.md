# Churn Prediction Model

This project implements a churn prediction model using various machine learning algorithms including Logistic Regression, Decision Tree, Bagging Classifier, and Support Vector Classifier (SVC). The dataset used is the Churn Modelling dataset which contains information about customer churn.

## Prerequisites

Before running the project, make sure you have the following installed:

- Python 3.12
- Libraries: `numpy`, `pandas`, `matplotlib`, `seaborn`, `scikit-learn`

Install the required libraries by running:

bash
`pip install numpy pandas matplotlib seaborn scikit-learn`


# Bank Customer Churn Prediction

This project aims to predict customer churn for a bank using various machine learning models.

## Dataset

The dataset used in this project is `Churn_Modelling.csv`. It contains the following columns:

- `CustomerId`: Unique customer identifier
- `CreditScore`: Customer credit score
- `Geography`: Country of the customer
- `Gender`: Gender of the customer
- `Age`: Customer age
- `Tenure`: Number of years the customer has been with the bank
- `Balance`: Bank balance
- `NumOfProducts`: Number of bank products held by the customer
- `HasCrCard`: Whether the customer has a credit card
- `IsActiveMember`: Whether the customer is an active member
- `EstimatedSalary`: Estimated annual salary of the customer
- `Exited`: Whether the customer has exited the bank (target variable)

## Exploratory Data Analysis

- Visualized categorical and numerical columns using seaborn's countplot and boxplot.
- Checked for duplicated rows and missing values.
- Performed feature encoding using one-hot encoding for categorical columns such as Geography and Gender.

## Feature Engineering

The dataset is cleaned by:
- Dropping unnecessary columns like RowNumber, CustomerId, and Surname.
- Applying one-hot encoding on categorical variables: Geography and Gender.

## Correlation Heatmap

A correlation heatmap was generated to understand the relationship between features and the target (Exited).

```python
sns.heatmap(cm, annot=True, cmap='viridis')
```

## Model Training

We trained the dataset using four different machine learning models:

1. Logistic Regression
   - Train Accuracy: 79.39%
   - Test Accuracy: 78.63%

2. Decision Tree Classifier
   - Train Accuracy: 79.85%
   - Test Accuracy: 79.10%

3. Bagging Classifier (with Decision Tree as base estimator)
   - Train Accuracy: 79.85%
   - Test Accuracy: 79.10%

4. Support Vector Classifier (SVC)
   - Train Accuracy: 78.60%
   - Test Accuracy: 77.57%

## Usage

[Include instructions on how to run the project, install dependencies, etc.]

## Contributing

[Include guidelines for contributing to the project]

## License

[Include license information]
