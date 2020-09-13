# Sentiment-Analysis-Topic-Modeling-for-Hotel-Reviews
Web Scraping, Sentiment Analysis, Latent Dirichlet Allocation (LDA) topic modelling

## Table of Contents

1. [Installation](#Installation)
2. [Project Motivation](#Project-Motivation)
3. [Data Description](#Data-Description)
4. [Methodologies](#Methodologies)
5. [Results](#Results)

## Installation
There should be no necessary libraries to run the code here beyond the Anaconda distribution of Python. 

## Project Motivation
The project goal is to use data mining techniques to analyze hotel reviews and help the hotel to identify factors that influence guest satisfactions.

## Data Description
I scraped reviews of "Hotel Beresford" (located in San Francisco, CA) from booking.com. The link of the hotel's review page is https://www.booking.com/reviews/us/hotel/beresford.html?

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

## Methodologies
* Exploratory Data Analysis
* Web Scraping (Requests and Beautiful Soup) 
* Text Analytics
   * WordCloud
   * Sentiment Analysis
   * Latent Dirichlet Allocation (LDA) topic modelling

## Reseults
Hotel Beresford needs to improve hotel guest satisfaction by providing friendlier services and work on issues related to soundproofing, air conditioning, shower system and parking. The hotel also need to work on improving guests satisfaction towards the breakfast they provide, maybe coffee or pastries as appeared in the WordCloud.  
All the visualizations provided in the exploratory data analysis as well as the pyLDAvis interactive visualization would help the hotel manager to further understand what most popular topics within the negative reviews are and make improvements accordingly.

