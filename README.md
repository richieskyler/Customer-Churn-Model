# PowerCo Churn Prediction Model

## Project Overview

This project aims to predict customer churn for PowerCo Analytics by performing comprehensive data analysis, cleaning, feature engineering, and model training. Two machine learning models, Decision Tree and Random Forest, were trained and tested to determine their effectiveness in predicting churn. Additionally, strategies were implemented to address dataset imbalance.

## Table of Contents

- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
- [Data Cleaning](#data-cleaning)
- [Feature Engineering](#feature-engineering)
- [Key Features Contributing to Churn](#key-features-contributing-to-churn)
- [Model Training and Evaluation](#model-training-and-evaluation)
  - [Handling Imbalanced Data](#handling-imbalanced-data)
  - [Decision Tree Model](#decision-tree-model)
  - [Random Forest Model](#random-forest-model)
- [Results](#results)
- [Conclusion](#conclusion)

## Dataset

The dataset used for this project contains customer information and their churn status. The key attributes include demographic details, account information, and usage patterns.

## Exploratory Data Analysis (EDA)

During the EDA phase, the following analyses were performed:

- Distribution of key features
- Correlation analysis between features
- Identification of missing values and outliers
- Visualizations to understand patterns and trends

## Data Cleaning

The dataset was cleaned to ensure accuracy and reliability by:

- Handling missing values
- Removing or correcting outliers
- Standardizing data formats

## Feature Engineering

Feature engineering involved creating new features and transforming existing ones to improve model performance. Key steps included:

- Creating new features based on domain knowledge
- Encoding categorical variables
- Normalizing numerical features

## Key Features Contributing to Churn

Through feature importance analysis, the following key features were identified as significant contributors to customer churn:

- **Net margin and consumption over 12 months**: A top driver for churn in this model.
- **Margin on power subscription**: An influential driver for churn.
- **Time-related factors**: The number of months customers have been active (tenure) and the number of months since they updated their contract are significant influencers.
- **Price sensitivity features**: Scattered around and not the main driver for a customer churning.

From this chart, we can observe the following points:

- Net margin and consumption over 12 months is a top driver for churn in this model.
- Margin on power subscription also is an influential driver.
- Time seems to be an influential factor, especially the number of months they have been active, their tenure, and the number of months since they updated their contract.
- Our price sensitivity features are scattered around but are not the main driver for a customer churning. 

The last observation is important because this relates back to our original hypothesis.

## Model Training and Evaluation

### Handling Imbalanced Data

To address the class imbalance in the dataset, techniques such as SMOTE (Synthetic Minority Over-sampling Technique) were used.

### Decision Tree Model

The Decision Tree model was trained and evaluated, achieving reasonable accuracy and recall rates. Key steps included:

- Splitting the data into training and testing sets
- Training the model on the training set
- Evaluating performance on the testing set

### Random Forest Model

The Random Forest model was trained and optimized, resulting in higher accuracy and recall rates. Key steps included:

- Splitting the data into training and testing sets
- Training the model on the training set
- Tuning hyperparameters for optimal performance
- Evaluating performance on the testing set


## Conclusion

The Random Forest model outperformed the Decision Tree model in predicting customer churn, demonstrating higher precision and recall rates. This project highlights the importance of thorough data analysis, cleaning, and feature engineering in building effective predictive models. Future work may involve exploring other machine learning algorithms and further optimizing feature selection.
