# Tweets-Semantic-Analysis
Semantic Analysis of Twitter data - whether Tweets are Racist/Sexist or Non-Racist/ Non-sexist

# Using Bagging and Boosting Techniques.

### Steps:
1. Read Train and Test datasets, which is already splitted into 2 seperate csv files.
2. EDA of length of tweets, in terms of words, in both train and test data
3. Data Cleaning: 
  
  Following steps are followed to clean text from data-

     - Removed twitter handles as they are already masked as @user due to privacy concerns. These twitter handles hardly give any information about the nature of the tweet.

     - Get rid of the punctuations, numbers and even special characters since they wouldn’t help in differentiating different types of tweets.

     - Most of the smaller words do not add much value. For example, ‘pdx’, ‘his’, ‘all’. So, we will try to remove them as well from our data.

     - Then, Text Normalization. For example, reducing terms like loves, loving, and lovable to their base word, i.e., ‘love’.are often used in the same context. If we can reduce them to their root word, which is ‘love’. It will help in reducing the total number of unique words in our data without losing a significant amount of information.
    
   - Story Generation and Visualization from Tweets- 
    - Word Cloud:
    
    i.
    ii.
    iii.
   4. Understanding the impact of Hashtags on tweets sentiment

      - Hashtags in twitter are synonymous with the ongoing trends on twitter at any particular point in time. 
      - We should try to check whether these hashtags add any value to our sentiment analysis task, i.e., they help in distinguishing tweets into the different sentiments.

      - For instance, given below is a tweet from our dataset:
      "what has today's attitude to women got in common with that of normal baites? #psycho #feminism #hollaback"
      The tweet seems sexist in nature and the hashtags in the tweet convey the same feeling.
   
      - Now that we have prepared our lists of hashtags for both the sentiments, we can plot the top ‘n’ hashtags.
      - Plot of non-racist/non-sexist tweets.
      
      - Plot of racist/sexist tweets.
      
   5. Information Retrieval from Natural Language Processing models- 
       Bag of Words-
       i. COunt Vectorizer 
       ii. Tf-Idf Vectorizer
      iii. word2vec
      iv. doc2vec
  
  6.. Modeling-
    Will use these 4 models-
     i. Logistic Regression
     ii. Support Vector Machine (SVM)
     iii. Random Forest
     iv. XGBoost
 
 F-1 scores of all models(without hyperparameter tuning)-
 
 7. As, it can be seen that, XGBoost model, with Word2Vec performs best. Performed hyperparameter tuning on XGBoost model-
 And got 70.3% accuracy as F-1 score.
      
      

    
