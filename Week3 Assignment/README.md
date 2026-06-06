MyName - Emmanuel Onwuhafua.

CourseName - MBAI5310G-AI-Programming.

RepositoryDescription - This repository is dedicated to my Ontario Tech AI Programming Lab and will be used for my weekly assignments and final project.

Note: This repository is dedicated to my Ontario Tech AI Programming Lab and will be used for my weekly assignments and final project.

*
*

# 1. Which model performed better?
ANSWER: The SVM model performed better overall, especially for the upgrade (“Yes”) class, because it achieved higher accuracy (0.82 vs 0.77), higher precision (0.71 vs 0.45), and a higher F1-score (0.43 vs 0.37).

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
Also, the model only uses historical features (revenue, tickets, product usage, etc.). It does not know the following; Current negotiations or relationships, Special deals, discounts, or strategic accounts, 
# Qualitative signals (tone in calls, emails, long-term relationship value)

