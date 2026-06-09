MyName - Emmanuel Onwuhafua.

CourseName - MBAI5310G-AI-Programming.

RepositoryDescription - This repository is dedicated to my Ontario Tech AI Programming Lab and will be used for my weekly assignments and final project.

Note: This repository is dedicated to my Ontario Tech AI Programming Lab and will be used for my weekly assignments and final project.

*
*

# Assignment 3: Classification Models and Evaluation Metrics 

# What problem is the business trying to solve?
The business wants to identify which customers are most likely to upgrade their current account plan. Rather than contacting every customer, the company wants to focus its marketing and sales efforts on customers who have a higher probability of upgrading.

# What decision can machine learning help the business make?
Machine learning can help predict whether a customer is likely to upgrade their account in the future. Using customer characteristics such as company size, annual revenue, monthly transactions, product usage score, account age, and training attendance, the model can classify customers as likely or unlikely to upgrade.

This allows the business to decide:
•	Which customers should be targeted by the sales team. 
•	Which customers should receive promotional offers. 
•	Which customers may benefit from additional training or engagement activities. 
•	How to allocate marketing resources more effectively. 

# Why is this prediction useful for the business?
Predicting account upgrades provides several business benefits:
1. Increased Revenue
The company can focus on customers with a higher likelihood of upgrading, increasing the chances of generating additional subscription revenue.
2. Improved Marketing Efficiency
Instead of spending money on broad marketing campaigns, the business can target specific customers who are more likely to respond positively.
3. Better Use of Sales Resources
Sales representatives can prioritize high-potential customers, reducing wasted effort on accounts that are unlikely to upgrade.
4. Improved Customer Retention and Engagement
Customers showing strong product usage or engagement can be identified early and encouraged to move to higher-tier plans that better meet their needs.
5. Data-Driven Decision Making
Rather than relying on intuition, management can use predictive insights to make more informed business decisions.

# Dataset used: 
business_account_upgrade_prediction_dataset

# Input Features:
Company_Size, Industry, Annual_Revenue, Monthly_Transactions, Current_Plan, Account_Age_Months, Support_Tickets, Sales_Contacted, Product_Usage_Score, Monthly_Fee, Training_Attended

# Target variable: 
Upgraded_Account

# Models used:
The models used are Logistic Regression and SVM.

# Task 1: Train and compare two classification models
Using one of the provided datasets, train two classification models:
•	Logistic Regression
•	SVM
For both models, calculate:
Confusion matrix
Accuracy
Precision
Recall
F1-score

<img width="1003" height="280" alt="image" src="https://github.com/user-attachments/assets/01188939-499f-4c4b-be55-7b561a15f1d9" />

# Task 2

# 1. Which model performed better?
ANSWER: The SVM model performed better overall, especially for the upgrade (“Yes”) class, because it achieved higher accuracy (0.82 vs 0.77), higher precision (0.71 vs 0.45), 
# 2. Which metric is most important for your business problem?
My most important metric is the F1-score for the “Yes” class, because we want to identify real upgrade opportunities without wasting too much sales and marketing effort on customers who will not upgrade.

# 3. What do false positives and false negatives mean in your dataset?
For SVM, using labels [“No”, “Yes”]:
We had 2 False Positives (FP = 2): predicted “Yes” but the actual is “No”. The model says a customer is likely to upgrade, but they actually don’t.
This meant that Business /marketing may spend time and budget contacting these customers, but get no upgrade. This indicates wasted sales time, marketing cost, possible customer annoyance.

We had 11	False Negatives (FN = 11): predicted “No” but the actual is “Yes”. The model says a customer is unlikely to upgrade, but they actually would have.
Hence, these customers may not be targeted or prioritized, so Business/ Marketting will miss out on potential upgrades and revenue. This indicates loss of revenue opportunities and weaker customer engagement.


# 4. What is one possible limitation or bias in your model?
One key limitation is class imbalance and limited data: there are many more “No” than “Yes” examples, so the model learns to predict “No” much more confidently. This can bias it against correctly identifying potential upgraders, especially in underrepresented customer segments.


# 5. Why should human judgment still be used?
Human judgment should still be used because the model cannot capture all the contextual, qualitative, and strategic information that sales and the Business have. Humans are needed to interpret the predictions, override them when necessary, and ensure that important customers and edge cases are handled appropriately, rather than relying solely on historical patterns.
Also, the model only uses historical features (revenue, tickets, product usage, etc.). It does not know the following; Current negotiations or relationships, Special deals, discounts, or strategic accounts, Qualitative signals (tone in calls, emails, long-term relationship value)
