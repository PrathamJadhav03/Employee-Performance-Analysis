# Employee Performance Analysis and Prediction

## Introduction

This project aims to analyze and predict employee performance using machine learning techniques. The dataset used in this project contains various features related to employee demographics, educational background, job details, and performance ratings. The analysis involves data preprocessing, exploratory data analysis (EDA), feature engineering, and modeling using different algorithms.

## Data Preprocessing

The code starts by importing the necessary libraries for data manipulation, visualization, and machine learning tasks. It then loads the dataset into a pandas DataFrame and performs the following preprocessing steps:

**1. Handling Missing Values:** The code checks for missing values in the dataset and finds that there are no missing values.

**2. Encoding Categorical Variables:** Categorical variables like 'Gender', 'EducationBackground', 'MaritalStatus', 'EmpDepartment', 'EmpJobRole', 'BusinessTravelFrequency', and 'OverTime' are encoded using various techniques such as label encoding, frequency encoding, and manual encoding.

**3. Handling Outliers:** The code identifies and imputes outliers in numerical features like 'TotalWorkExperienceInYears', 'TrainingTimesLastYear', 'ExperienceYearsAtThisCompany', 'ExperienceYearsInCurrentRole', 'YearsSinceLastPromotion', and 'YearsWithCurrManager' using the Interquartile Range (IQR) method.

**4. Feature Transformation:** The 'YearsSinceLastPromotion' feature is transformed using square root transformation to handle skewness.

**5. Feature Scaling:** Numerical features are scaled using the StandardScaler from scikit-learn to ensure they are on the same scale.

**6. Feature Selection:** The code performs feature selection by dropping unique and constant features, checking for high correlation among features, and employing Principal Component Analysis (PCA) to reduce the dimensionality of the dataset.

**7. Saving Preprocessed Data:** The preprocessed data is saved as a CSV file for further analysis and modeling.

## Exploratory Data Analysis (EDA)

The code performs a comprehensive EDA to understand the dataset better and gain insights into the relationships between different features and the target variable (PerformanceRating). The EDA includes:

**1. Domain Analysis:** Understanding the meaning and impact of each feature on the target variable.

**2. Statistical Analysis:** Calculating summary statistics for numerical and categorical features.

**3. Univariate Analysis:** Visualizing the distribution of individual features using histograms and bar plots.

**4. Bivariate Analysis:** Analyzing the relationship between two features and the target variable using line plots and bar plots.

**5. Multivariate Analysis:** Exploring the relationships between multiple features and the target variable using various visualizations such as line plots, bar plots, and violin plots.

The EDA section also includes checks for skewness, kurtosis, and distribution of mean and standard deviation of the data.

## Modeling and Evaluation

The code splits the preprocessed data into training and testing sets and balances the target variable using the SMOTE (Synthetic Minority Over-sampling Technique) technique. It then trains and evaluates three different machine learning models:

**1. Support Vector Machine (SVM):** The code trains an SVM model and evaluates its performance on the training and testing sets using metrics such as accuracy, precision, and classification report.

**2. Random Forest Classifier:** A Random Forest Classifier is trained, and its performance is evaluated. The code also performs hyperparameter tuning using RandomizedSearchCV to improve the model's performance.

**3. Artificial Neural Network (Multilayer Perceptron Classifier):** An Artificial Neural Network model is trained and evaluated using various metrics.

The code compares the performance of these three models and selects the best-performing model based on the evaluation metrics.

## Saving the Model

The code saves the best-performing model (Multilayer Perceptron Classifier) using the pickle library for future use.

## Conclusion

The GitHub post provides a detailed overview of the code, covering data preprocessing, exploratory data analysis, modeling, and evaluation steps. It highlights the various techniques and algorithms used in the project and showcases the in-depth analysis performed on the employee performance dataset.

Note: This GitHub post assumes that the reader has a basic understanding of machine learning concepts and Python programming. The post aims to provide a high-level overview of the code and its functionality.
