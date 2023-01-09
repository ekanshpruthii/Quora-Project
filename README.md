# Quora-Project
The dataset originally consists of question pairs, ids and if the pair is duplicate or not. 
<img width="828" alt="image" src="https://user-images.githubusercontent.com/110238036/211220191-7c58ba2f-cb7e-482b-bdd3-e693ee7f5680.png">

There are total of 404,290 records in raw data. 
Now the data is not in its perfect form hence it requires the extensive preprocessing before we start applying machine learning algorithms.
There is proper EDA done on the dataset where there are many more columns being introduced in the dataframe.
<img width="994" alt="image" src="https://user-images.githubusercontent.com/110238036/211220397-eaa429e6-1bfc-4fda-9ca4-7f6389c84b03.png">
Total columns now stands at 32 which would be very useful when we apply the NLP techniques or Machine Learning Models.

During EDA, while trying dimension Reduction technique the result showed that there is no good result that can be seen after applying PCA technique hence decided to remove it.
Graphical representation of the same is:
<img width="980" alt="image" src="https://user-images.githubusercontent.com/110238036/211229969-70b99ce4-16f9-439a-bda5-00424533a363.png">

Next used the TF-IDF scores, converted each question to a weighted average of word2vec vectors by these scores.
next used a pre-trained GLOVE model which comes free with "Spacy". It is trained on Wikipedia and therefore, it is stronger in terms of word semantics.

Next task is to apply Machine learning algorithms to predict if the question pair is duplicate or not. While trying to apply various algorithms such as Decision tree,Logistic Regression, SVM, KNN, Random Forest.
<img width="1003" alt="image" src="https://user-images.githubusercontent.com/110238036/211231658-2d20bcc6-1d89-4506-a3af-4ce73d63d44f.png">
<img width="989" alt="image" src="https://user-images.githubusercontent.com/110238036/211231668-4b4fb4f3-9633-4a2d-a642-368d497be827.png">
<img width="1000" alt="image" src="https://user-images.githubusercontent.com/110238036/211231689-7feaf012-1536-4fe3-94c1-9fe3c0df7932.png">
<img width="1007" alt="image" src="https://user-images.githubusercontent.com/110238036/211231724-60b6914b-9998-465d-9d4d-e2eac605ca31.png">
<img width="998" alt="image" src="https://user-images.githubusercontent.com/110238036/211231734-5ebdd15e-c91b-4603-9eb6-712b0d4359e9.png">

<h2>The best one came out to be Gradient Boosting:</h2>
<img width="989" alt="image" src="https://user-images.githubusercontent.com/110238036/211231777-176db211-1205-4e35-99b3-328cfe6b0d0f.png">

