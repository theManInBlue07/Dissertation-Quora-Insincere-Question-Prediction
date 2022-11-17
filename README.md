# Dissertation-Quora-Insincere-Question-Presiction

Project Aim/Objective
To develop Deep Learning Models to identify or weed out insincere questions on platforms like Quora .
Quora is a platform that empowers people to learn from each other. On Quora, people can ask questions and connect with others who contribute unique insights and quality answers. A key challenge is to weed out insincere questions — those founded upon false premises, or that intend to make a statement rather than looking for helpful answers.

What is an Insincere Question ?
A question is said to be Insincere if it based on any of the listed metrics :
● It has a non-neutral tone.
● It is disparaging or inflammatory.
● It isn’t grounded on reality.
● Uses sexual content(bestiality, phedophilia and incest) for shock value and not
seeking genuine answers.
My aim is to predict whether a question asked on Quora is insincere or not so that users can feel safe on their platform.


Project Objectives/Deliverables:
The objectives of the project are mentioned below:
● To collect text data consisting of qid- unique question identifier,question_text - Quora question text and target - a question labeled “insincere” having a value of 1, otherwise 0.
● To clean data, further preprocessing the data by implementing techniques in NLP
● To select important features for text featurization which are important for the analysis of data.
● Using word embedding techniques like Word2vec , Glove,Paragram and Wiki_news for creating word embeddings to understand the distributional Semantics of words in Natural Language processing.
● The model is based on bidirectional LSTM and GRU with attention,state of art BERT which uses Transformers to make the model more accurate with different embedding and features.
● Training the state of art Bert Model and predicting the result using F1-Score.
● Training the Model on the training dataset and testing the efficiency of the model using F1 score metric on test data and cross validation data.



Methodology:
The dataset consists of Questions framed in English which is used as a medium to share knowledge , views , critics , emotion across all the platforms in this world. Computers only understand binary language. In order to make sense of our data we need to transform the text information to vectors so that Data could be visualized and analyzed better.
The train dataset has 1,300,000 labeled data points labeled as Insincere or not . The
train dataset has 300,000 unlabeled data points. Some text featurization techniques to be implemented like removing special characters ,converting all words to lowercase letters etc.
● Tokenization - Breaking of texts into individual words called tokens.
● Stop word removal.
● Stemming - Breaking a word to its root|stem. Word may|may not belong to the
actual word in the dictionary of the language .
● Lemmatization - same process as Stemming . But the root words generated after
Lemmatization belong to the dictionary of the language .
● N-grams - Combination of multiple words used together to preserve sequential
information. 
Further using Word2Vec techniques to convert words to vectors. Using word embeddings our data is compared to 300 dimensional embeddings to better understand the semantic relation between words.
Developing the model bidirectional LSTM and GRU with attention and BERT and training it using the cleaned , preprocessed and vectorized data to evaluate the result using F1 score metric.
