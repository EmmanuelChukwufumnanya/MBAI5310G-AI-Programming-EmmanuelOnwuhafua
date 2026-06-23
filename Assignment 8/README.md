## Business Interpretation

The objective of this project was to develop a text classification model that can automatically categorize tourism visitor feedback into predefined service categories. The model is designed to predict the type of issue or experience being described in a visitor's comment, such as Ticketing, Food Service, Accessibility, Exhibit Experience, Staff Guidance, or Parking.
The dataset used in this study was the Tourism Visitor Feedback Dataset, which contains 120 visitor feedback records collected from different tourism channels and attraction areas. The primary text column selected for analysis was VisitorFeedback, while the target variable was FeedbackCategory, which represents the category of feedback provided by each visitor.

## Task 1: Load and Inspect the Dataset - Explain what each important column means.
The dataset contains tourism visitor feedback collected from different visitors and channels. The VisitorFeedback column contains the textual comments, while the FeedbackCategory column identifies the type of issue or experience being described. The target variable is perfectly balanced because each category contains the same number of records. This helps reduce classification bias during model training.

## Task 2: Text Preprocessing - After preprocessing, explain how the text changed and why preprocessing is important.
Text preprocessing helps standardize the data before analysis. Converting text to lowercase ensures that words such as "Ticket" and "ticket" are treated as the same word. Removing punctuation and stopwords eliminates unnecessary information that does not contribute meaningfully to classification. Tokenization breaks sentences into individual words, while stemming or lemmatization reduces words to their root forms. These steps improve the quality of the features used by the machine learning model.

## Task 3: Exploratory Text Analysis - Explain what the frequent words tell you about the dataset and the business problem.
The most common words provide insight into the issues visitors discuss most frequently. Words such as "ticket," "line," and "machine" suggest recurring concerns related to ticketing services. Words like "staff" and "group" indicate discussions involving visitor assistance and guided experiences. The frequent occurrence of "parking" highlights transportation and accessibility concerns. These patterns help identify areas where tourism management may need to improve visitor services

## Task 4: POS Tagging and Named Entity Recognition - 
Which words are nouns, verbs, or adjectives
Whether any names, locations, brands, organizations, or dates were detected
How this information could be useful in business text analysis - 

The Named Entity Recognition (NER) can identify entities such as:
NER can help tourism managers identify frequently mentioned locations, attractions, or organizations within visitor feedback. This allows organizations to monitor public perception of specific attractions and services more effectively.

## Task 5: Feature Extraction - Explain why text must be converted into numbers before using a machine learning model.
Machine learning algorithms cannot directly understand text. Therefore, text must be converted into numerical values before model training. TF-IDF converts words into numerical features by measuring how important each word is within a document relative to the entire dataset. This helps the model focus on meaningful words while reducing the influence of commonly occurring words

## Task 6: Build a Text Classification Model - 
The model learns patterns between visitor comments and their associated feedback categories. It then uses these patterns to predict the category of new visitor feedback. Logistic Regression is a suitable baseline model because it is simple, efficient, and performs well for text classification problems.

## Task 7: Model Evaluation - 
Results
Accuracy: 100%
Precision: 100%
Recall: 100%
F1-Score: 100%
Interpretation

The model correctly classified all records in the testing dataset. This suggests that the feedback categories are highly distinguishable based on the words used in the visitor comments. However, such perfect performance may also indicate that the dataset is relatively small and contains clearly separated categories. In a real-world environment with more diverse feedback, performance may be lower.
