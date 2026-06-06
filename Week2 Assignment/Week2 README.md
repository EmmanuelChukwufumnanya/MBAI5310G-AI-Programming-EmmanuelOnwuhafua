MyName - Emmanuel Onwuhafua.

CourseName - MBAI5310G-AI-Programming.

RepositoryDescription - This repository is dedicated to my Ontario Tech AI Programming Lab and will be used for my weekly assignments and final project.

Note: This repository is dedicated to my Ontario Tech AI Programming Lab and will be used for my weekly assignments and final project.



# What your model is trying to predict.  
ANSWER: It's trying to predict if a customer will upgrade their business account (Upgraded_Account = Yes or No).


# What dataset you used. 
ANSWER: I used a dataset of 377 business accounts, each with information such as company size, industry, revenue, product usage, support tickets, and whether they eventually upgraded. 
After cleaning, I removed 7 duplicate rows and handled missing values in several columns. I ended up with 370 rows and 13 columns. Originally the target had 293 -No- and 84 -Yes-.

# What features and target you selected.
ANSWER: Categorical Features: Company_Size, Industry, Current_Plan, Sales_Contacted, Training_Attended.
Numerical Features: Annual_Revenue, Monthly_Transactions, Account_Age_Months, Support_Tickets, Product_Usage_Score, Monthly_Fee.
Target: Upgraded_Account.

# What result you obtained.  
ANSWER: I achieved an Accuracy of 77.0% using the logistic regression model.
That means about 70% of test predictions matched the true labels.
 

# One limitation of your model or dataset
ANSWER: There are far fewer -Yes- cases than -No- (class imbalance). 
High accuracy can hide poor performance on the minority class — the model might still miss many real upgraders.
