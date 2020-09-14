# Sentiment-Analysis-Topic-Modeling-for-Hotel-Reviews
Web Scraping, Sentiment Analysis, Latent Dirichlet Allocation (LDA) topic modelling

## Table of Contents

1. [Installation](#Installation)
2. [Project Overview](#Project-Overview)
3. [Problem Statement](#Problem-Statement)
4. [Methodologies](#Methodologies)
5. [Data Description](#Data-Description)
6. [Results](#Results)
7. [Blog Post](#Blog-Post)

## Installation
There should be no necessary libraries to run the code here beyond the Anaconda distribution of Python. 

## Project Overview
In this project, I scraped hotel reviews of “Hotel Beresford” located in San Francisco, CA from the website bookings.com. Then, I did some data exploration, generated WordClouds, performed sentiment analysis and created an LDA topic model

## Problem Statement
The project goal is to use text analytics and Natural Language Processing (NLP) to extract actionable insights from the reviews and help the hotel improve their guest satisfactions.

## Methodologies
1) **Web Scraping:**
The hotel reviews were scraped from bookings.com by using requests with BeautifulSoup. 

2) **Exploratory Data Analysis (EDA):**
This part contais a pie chart, a histogram, and a seaborn violin plot to get a better understanding of the overall reviews and ratings.

3) **WordClouds:**
In order to generate more meaningful WordClouds, I customized extra stop words and used lemmatization to remove closely redundant words.

4) **Sentiment Analysis:**
The sentiment analysis helps to classify the polarity and subjectivity of the overall reviews and determine whether the expressed opinion in the reviews is mostly positive, negative, or neutral.

5) **LDA Topic Model:**
In natural language processing, the latent Dirichlet allocation is a generative statistical model that allows sets of observations to be explained by unobserved groups that explain why some parts of the data are similar. I used GridSearch to find the best topic model. The two tuning parameters are: (1) n_components: number of topics and (2) learning_decay (which controls the learning rate)

## Data Description
I scraped the data from the hotel review page: https://www.booking.com/reviews/us/hotel/beresford.html?

The scraped data are stored under 3 dataframes:
1) **reviewer_info**: Basic information of the reviewer and reviews:
    * Rating Score
    * Reviewer Name
    * Reviewer's Nationality
    * Overall Review (contains both positive & negative reviews)
    * Reviewer Reviewed Times
    * Review Date
    * Review Tags (Trip type, such as business trip, leisure trip, etc.)
2) **pos_reviews**Positive reviews
3) **neg_reviews**egative reviews

## Results
Hotel Beresford needs to improve hotel guest satisfaction by providing friendlier services and work on issues related to soundproofing, air conditioning, shower system and parking. The hotel also need to work on improving guests satisfaction towards the breakfast they provide, maybe coffee or pastries as appeared in the WordCloud.  
All the visualizations provided in the exploratory data analysis as well as the pyLDAvis interactive visualization would help the hotel manager to further understand what most popular topics within the negative reviews are and make improvements accordingly.

## Blog Post
If you are interested in reading my blog post about this project, please visit [Medium](https://medium.com/@jwbusiness123/sentiment-analysis-topic-modeling-for-hotel-reviews-6b83653f5b08?source=friends_link&sk=6bb2c73a2cfc5045ae528c9a5e823ceb)

