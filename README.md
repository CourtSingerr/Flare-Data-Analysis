# -Intro-to-Machine-Learning-Final-Project

Solar Flare Prediction Project
Project Overview
This project aims to analyze and model solar flare data to predict the occurrence of different classes of solar flares (C-Class, M-Class, X-Class). The dataset, sourced from the UCI Machine Learning Repository, consists of various features representing solar activity. The goal is to use this data to build robust predictive models.

Data Cleaning and Preprocessing
The data cleaning process involved several key steps to ensure the dataset was suitable for analysis and modeling:

Basic Data Cleaning:

Corrected the structure of the dataset.
Verified and converted variable types.
Checked for and handled missing data.
Outlier Detection and Management:

Used the Interquartile Range (IQR) method to identify outliers.
Retained outliers to preserve data integrity, employing robust scaling to mitigate their impact.
Data Scaling:

Applied a robust scaler to the target variables.
Imbalance Detection:

Identified significant class imbalances.
Combined target variables to create more balanced categories.
Data Transformation:

Applied Box-Cox transformation to reduce skewness.
Encoding Categorical Data:

Applied one-hot encoding to represent categorical data numerically.
Exploratory Data Analysis (EDA)
The EDA provided insights into the underlying patterns and distributions within the data:

Descriptive Statistics:

Calculated descriptive statistics for categorical features and target variables.
Visualizations:

Created count plots for categorical features and compared distributions of target variables before and after transformations.
Kolmogorov-Smirnov Test:

Performed to compare the distribution of C-Class flares to an exponential distribution, indicating the need for different modeling approaches.
Modeling
The modeling process involved several steps and the use of various machine learning models:

Data Splitting:

Split the data into training and test sets using stratified sampling.
Baseline Model:

Used linear regression as a baseline to provide initial performance insights.
Advanced Models:

Implemented Random Forest and Gradient Boosting models, which significantly outperformed the baseline.
Feature Selection:

Evaluated feature importance using Random Forest and Recursive Feature Elimination (RFE).
Class Imbalance Handling:

Applied SMOTE (Synthetic Minority Over-sampling Technique) to balance the target variable distributions.
Model Evaluation:

Evaluated models using Mean Squared Error (MSE) and compared performance across different preprocessing techniques.
Final Model and Findings
Advanced Models: Random Forest and Gradient Boosting models provided the best performance.
Data Transformation: The Box-Cox transformation was effective in reducing skewness and improving model performance.
Feature Importance: Key features identified included ZurichClass, SpotSize, Activity, Evolution, and Prev24hrFlare.
Class Imbalance: Addressed using SMOTE, leading to better performance on minority classes.
