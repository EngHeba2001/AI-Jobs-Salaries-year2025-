AI Jobs & Salaries 2025–2026 – Project Summary

This project analyzes a dataset of 1,500 AI job postings from 2025–2026 and builds a Multi-Output Classification Model to predict three targets simultaneously:

Salary Tier
Benefits Score Level
Demand Growth Level
Data Preparation
No missing values or duplicate records were found.
Unnecessary columns and potential leakage features were removed.
The required_skills column was transformed into 93 binary skill features using one-hot encoding.
Experience level and company size were cleaned and standardized.
Numerical targets were converted into categorical classes for classification.
Model

A CatBoost Classifier was used within a MultiOutputClassifier framework, with Multilabel Stratified K-Fold validation to preserve class distributions across all target variables.

Results
Target	Test Accuracy
Salary Tier	90.4%
Benefits Score Level	76.4%
Demand Growth Level	65.6%–86%
Overall Accuracy	84.3%
Key Insights
Salary tier can be predicted with very high accuracy using job characteristics, skills, and experience.
Benefits score is more difficult to predict due to class imbalance.
Demand growth prediction achieved reasonable performance using market demand indicators and skill requirements.
CatBoost proved effective for handling mixed numerical and categorical data with minimal preprocessing.
Technologies Used

Python, Pandas, NumPy, Scikit-Learn, CatBoost, Matplotlib, Seaborn, and Iterative Stratification.

Conclusion

The developed multi-output machine learning model successfully predicts salary level, benefits quality, and demand growth for AI-related jobs, providing valuable insights into labor market trends and career opportunities in the AI industry.
