MyName - Emmanuel Onwuhafua.

CourseName - MBAI5310G-AI-Programming.

RepositoryDescription - This repository is dedicated to my Ontario Tech AI Programming Lab and will be used for my weekly assignments and final project.

Note: This repository is dedicated to my Ontario Tech AI Programming Lab and will be used for my weekly assignments and final project.



**Week 4A ProcurePro Office Supplies**

Business Problem

ProcurePro Office Supplies relies on multiple suppliers to fulfill customer purchase orders. Supplier delivery delays can result in inventory shortages, operational disruptions, emergency purchases, and reduced customer satisfaction. The objective of this project is to predict whether a purchase order is at high risk of supplier delivery delay.

Dataset

The dataset contains 360 purchase order records and includes supplier information, order characteristics, delivery conditions, supplier performance metrics, inventory information, and risk indicators. The target variable is Supplier_Delay_Risk, where: • Yes = High Risk of Supplier Delay • No = Low Risk of Supplier Delay

Machine Learning Model

A Decision Tree Classification model was developed using Scikit-Learn. Categorical variables were converted using One-Hot Encoding, and the dataset was split into training and testing sets using an 80/20 ratio.

Main Evaluation Results

• Training Accuracy: 86.81% • Testing Accuracy: 68.06% • Precision: 73.81% • Recall: 72.09% • F1-Score: 72.94%

Key Business Insights

The model successfully identifies many high-risk supplier orders and can serve as an early-warning system for procurement managers. Important risk indicators include supplier reliability, historical delays, backorder history, supplier ratings, and inventory buffer levels.

Limitation

The dataset is synthetic and may not fully reflect real-world supplier behavior. Additionally, external factors such as weather disruptions, transportation issues, and market conditions are not captured by the model.
