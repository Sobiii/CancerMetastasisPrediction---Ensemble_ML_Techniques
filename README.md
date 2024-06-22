# Predicting Cancer Metastasis Period with Stacked Ensemble Models

## Overview

This project utilises the WiDS dataset consisting of over 100 features to create a stacked ensemble model for predicting the metastasis period of breast cancer (how long after diagnosis cancer metastasises). Due to the extensive number of features, the project involved domain research, extensive exploratory data analysis (EDA), and meticulous preprocessing to handle missing values.

## Key Features

- **Domain Knowledge Integration**: Leveraging domain research to select and engineer features.
- **Exploratory Data Analysis**: Comprehensive correlation analysis and visualisations to understand data relationships.
- **Feature Engineering**: Creating new features from existing ones to enhance model performance.
- **Advanced Preprocessing**: Handling a large number of missing values with careful imputation techniques.
- **Innovative Residual-Based Feature**: Using model residuals to calculate prediction error probabilities, which are used as an additional feature in the final predicting model.
- **Stacked Ensemble Model**: Combining multiple base learners with a meta-learner for improved predictions.

## Model Structure

### Base Learners

1. **CatBoost**
2. **Linear Regression Model**
3. **Random Forest Regressor**
4. **Support Vector Regressor**
5. **Extreme Random Trees**
6. **FeedForward Neural Network**
7. **AdaBoost**
8. **Elastic Net**

### Meta-Learner

- **Linear Regression**

### Innovative Approach

An innovative approach was employed where the model's predictions were used to calculate residuals. These residuals were then normalised to determine prediction error probabilities, which were subsequently used as an additional feature in the final predicting model. This method enhances the model's ability to understand and correct its own errors, leading to more accurate predictions.

## Results

The stacked ensemble model demonstrates high accuracy in predicting the metastasis period of breast cancer. The innovative approach of using residual-based features significantly enhances the model's predictive capability. Detailed performance metrics and visualisations are provided in the evaluation notebook.

