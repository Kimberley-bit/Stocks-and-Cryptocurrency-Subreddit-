# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) Project 2: Stocks and Cryptocurrency

## Problem Statement ##
This project aims to apply machine learning techniques to curate and flag irrelevant content posts within each subreddit so as to improve the quality of users’ experience and grow the active user base for better advertising revenue potential. In classifying the posts, we also want to mitigate the risk of losing users to inappropriate removal of posts when they are actually relevant to the thread.

## Datasets used ##
1. Stock Subreddit Thread
   - Created Jun 27, 2008
   - 3 million followers
2. Cryptocurrency Subreddit Thread
   - Created Mar 11, 2013
   - 3.5 million followers

#### Chosen Data Cleaning Techniques using NLP: #### 
1. Remove Punctuation
2. Tokenisation
3. Remove Stopwords
4. Stemming
5. Lemmatize
     
#### Chosen EDA Techniques: ####
1. Vectorization
2. Word Count
3. Average words

#### Chosen Models: ####
1. Bernoulli Naive Bayes
2. Multinomial Naive Bayes
3. Gaussian Naive Bayes    
4. Logistic Regression
5. K-Nearest Neighbours
     
#### Results: ####
Logistic Regression was the chosen model in the end as it showed the best score for Count Vectorization as well as TF-IDF in testing and also after evaluation.

#### Recommendations: ####
1. Deploy the model for testing with live data
a. Given the strong performance of the model (96% accuracy score and 97% sensitivity score), we can benefit from deploying the model for pilot testing on the reddit platform. 
2. Flag posts classified as irrelevant for moderators' assessment
a. There is a risk of incurring user frustrations if relevant posts are removed as a result of the model misclassification. To minimize wrongful post(s) removal, we can use the model's recommendation to flag posts for moderators' consideration. 
3. Share keywords insights with the moderators
a. This can help moderators set rules for content posting using the AutoModerator to ensure irrelevant topics will not be posted within the community. 
        
#### Future Steps moving ahead: ####
1. Collect data samples across a longer time (e.g. the past year) for training and model optimisation to pre-empt risk that the topics of discussion and keywords may change across different times of the year. 
2. Train the data using irrelevant posts from more than one source.
3. Train and further optimise the model for production across more subreddit communities. 

## Jupyter Notebooks should be read in this order ##
Book   | Name
-------|-----------
(Bk 1) | Scrapping_Stocks_Final.ipynb
(Bk 2) | Scrapping_Crypto_Final.ipynb
(Bk 3) | Cleaning Data_Stocks.ipynb
(Bk 4) | Cleaning Data_Crypto.ipynb
(Bk 5) | Cleaning Data & EDA.ipynb
(Bk 6) | Modeling - Count Vectorization.ipynb
(Bk 7) | Modeling - TF_IDF.ipynb
