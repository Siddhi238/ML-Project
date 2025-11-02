# Machine Learning YouTube Sentiment Analysis.

# Problem Statement
The primary objective of the project is studying and categorizing user comments of YouTube videos as positive, negative or neutral. Nowadays, on the web, billions of comments are posted every day, via online platforms such as YouTube, these opinions can guide content authors and organizations to better engage their audiences, as well as filter harmful comments.
# Why It’s Important
In YouTube, the comments represent the true sentiment of the user. 
•	Detect spam or hate speech automatically.
•	Understand audience feedback on specific videos or topics.
•	Improve content moderation and personalization systems.
Overview of Results
The model was trained to identify good sentiments in comments. Findings indicate that the Logistic Regression and Naive Bayes models were most effective as far as the first-order classification of text was concerned, achieving an accuracy of approximately 85-90, depending on preprocesses and hyperparameters.




# Dataset Source
•	Source: Kaggle — YouTube Comments Dataset
•	Access Method:
•	 <img width="925" height="136" alt="image" src="https://github.com/user-attachments/assets/0920c5cb-1c09-4477-8f5e-cc26dcffa21b" />


•	Data Size: ~50,000 comments (varies by subset)
•	Key Columns:
o	COMMENT_ID — Unique ID for each comment
o	AUTHOR — Username of commenter
o	LIKES — Number of likes on the comment
o	REPLY_COUNT — Number of replies

# Preprocessing Steps
•	Eliminated redundant records and blank fields.
•	Lowercased all text.
•	Deleted punctuations, special characters
•	Words tokenized and Stemming / Lemmatization used
•	Split data into training and testing sets.





# Methods
# Approach
1.	Data Cleaning & Text Preprocessing
o	NLTK used in lemmatization, removal of stopwords and tokenization.
o	F-IDF Vectorization changed textual information into numerical attributes.
2.	Model Training
o	Logistic Regression, Naive Bayes and Random Forest trained models.
o	Evaluated each using accuracy, precision, recall, and F1-score.
3.	Visualization
o	Created word clouds for each sentiment class.
o	Assessed every one in terms of accuracy, precision, recall, and F1-score.

# Why This Approach?
•	Text data has the advantage of being represented with a more useful feature representation using text mining (TF-IDF).
•	Naive Bayes and Logistic regression are effective and explainable to sentiment analysis.
Alternative Approaches
•	Further improvement of accuracy could be made with Deep Learning with LSTM or BERT embeddings.
•	May exploit self-directed study on the topic






Steps to Run the Code
Import Dataset:
 <img width="903" height="120" alt="image" src="https://github.com/user-attachments/assets/4be9d368-4358-4632-82ce-c8cfe4600146" />


Load Data : 
 <img width="903" height="120" alt="image" src="https://github.com/user-attachments/assets/2af9e90c-60c8-4b6c-a303-6352ccae7b7e" />


1.	Preprocess Text:
o	Filter and purify comments.
o	Apply TF-IDF vectorization.
2.	Train Model:
o	Split dataset - Train models - Evaluate performance.
3.	Visualize Results:
4.	
MODEL	ACCURACY	PRECISION	RECALL 	F1- Score
Logistic Regression	89%	88%	87%	88%
Naive Bayes	87%	86%	85%	86%
Random Forest	84%	83%	82%	83%

# Observations:
•	The maximum accuracy was obtained with Logistic Regression
•	A word cloud analysis is used to indicate that positive comments have words such as love, amazing, awesome and negative with words such as worst, hate, and boring .
•	The data was rather skewed (there were more positive reviews than negative ones).

# Conclusion
•	Developed an effective sentiment analysis pipeline on Google comments
•	The Logistic Regression was the most suitable overall approximation between the accuracy and the simplicity.
•	The use of sophisticated deep learning models (LSTM, BERT) to understand the context can be incorporated in work in the future.


# References
1.	Kaggle Dataset: YouTube Comments Dataset – Atif Ali Ak
2.	NLTK Documentation – https://www.nltk.org/
3.	Scikit-learn Documentation – https://scikit-learn.org/
4.	WordCloud Library – https://amueller.github.io/word_cloud/
