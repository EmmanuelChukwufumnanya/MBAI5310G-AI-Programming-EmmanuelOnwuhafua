MyName - Emmanuel Onwuhafua.

CourseName - MBAI5310G-AI-Programming.

RepositoryDescription - This repository is dedicated to my Ontario Tech AI Programming Lab and will be used for my weekly assignments and final project.

Note: This repository is dedicated to my Ontario Tech AI Programming Lab and will be used for my weekly assignments and final project.




**Employee Attrition Prediction Using Decision Tree Classification**

Business Problem Employee attrition can lead to increased recruitment costs, loss of organizational knowledge, and reduced productivity. The objective of this project is to develop a machine learning model that predicts whether an employee is likely to leave the company so that HR teams can take proactive retention actions. Dataset Used

The TalentWise Employee Attrition dataset contains 360 employee records and 19 variables describing employee demographics, work conditions, performance, engagement, and satisfaction.

Target Variable: • Left_Company (0 = Stayed, 1 = Left)

Machine Learning Model Used

A Decision Tree Classifier was developed using Scikit-Learn.

Project steps included: • Data inspection and cleaning • Feature selection • One-Hot Encoding of categorical variables • Train-Test Split (80/20) • Decision Tree Classification • Model evaluation

Main Evaluation Results

Controlled Decision Tree Model: • Training Accuracy: 86.46% • Testing Accuracy: 79.17% • Precision: 84.13% • Recall: 91.38% • F1-Score: 87.60%

Overfitted Decision Tree Model: • Training Accuracy: 100.00% • Testing Accuracy: 72.22%

Key Business Insights

The model demonstrates that employee attrition can be predicted with reasonable accuracy.

Potential drivers of employee attrition include: • Employee engagement • Salary satisfaction • Manager support • Workload levels • Overtime hours • Career progression opportunities

These insights can help HR departments design targeted retention strategies and improve workforce planning. Model Limitation

The dataset contains only 360 employee records and has an imbalanced target distribution, with significantly more employees staying than leaving. This may limit the model's ability to generalize to new employee populations and may affect predicperformance for employees who leave the company.
