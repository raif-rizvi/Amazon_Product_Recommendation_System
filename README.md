# Amazon Style Product Recommendation System
This project focuses on building a recommendation system for Amazon. It utilizes various recommendation system models to suggest products to customers based on their previous ratings for other products.

## Table of Contents
- [Installation](#installation)
- [Project Motivation](#project-motivation)
- [File Descriptions](#file-descriptions)
- [Results](#results)
- [Licensing, Authors, and Acknowledgements](#licensing-authors-and-acknowledgements)

## Installation
The project is written in Python 3.7. Necessary libraries and their versions are:
- pandas
- numpy
- matplotlib
- seaborn
- scikit-surprise

## Project Motivation
Today, information is growing exponentially with volume, velocity and variety throughout the globe. This has lead to information overload, and too many choices for the consumer of any business. It represents a real dilemma for these consumers and they often turn to denial. Recommender Systems are one of the best tools that help recommending products to consumers while they are browsing online. Providing personalized recommendations which is most relevant for the user is what's most likely to keep them engaged and help business.

E-commerce websites like Amazon, Walmart, Target and Etsy use different recommendation models to provide personalized suggestions to different users. These companies spend millions of dollars to come up with algorithmic techniques that can provide personalized recommendations to their users.

Amazon, for example, is well-known for its accurate selection of recommendations in its online site. Amazon's recommendation system is capable of intelligently analyzing and predicting customers' shopping preferences in order to offer them a list of recommended products. Amazon's recommendation algorithm is therefore a key element in using AI to improve the personalization of its website. For example, one of the baseline recommendation models that Amazon uses is item-to-item collaborative filtering, which scales to massive data sets and produces high-quality recommendations in real-time.
### Scenario
You are a Data Science Manager at Amazon, and have been given the task of building a recommendation system to recommend products to customers based on their previous ratings for other products. You have a collection of labeled data of Amazon reviews of products. The goal is to extract meaningful insights from the data and build a recommendation system that helps in recommending products to online consumers. 

## File Descriptions
The repository contains the following file:
- `Amazon_Product_Recommendation_System.ipynb`: This is the Google Colab Notebook where all the work is done, which includes data loading, preprocessing, exploratory data analysis, model building, and evaluation.

## Dataset Information

The dataset employed for this project is comprehensive and offers the following insights:

- It contains a total of **7,824,481** entries.
- The three columns are: `'user_id'`, `'prod_id'`, and `'rating'`, none of which contain null values.
- The `'user_id'` column contains **4,201,696 unique** users, with the most frequent user being `'A5JLAU2ARJ0BO'`, who appears 520 times.
- The `'prod_id'` column contains **476,001 unique** products, with the most rated product being `'B0074BW614'`, receiving 18,244 ratings.
- Ratings in the `'rating'` column are integers ranging from 1 to 5. The most frequent rating is **5.0**, appearing 4,347,540 times.

### Sparse Nature of Recommendation Systems

Recommendation systems often deal with sparse data, mainly due to the large number of available items and the limited number of items each user has rated. This dataset is no exception, as the 7,824,481 entries represent only a tiny fraction of the 2,000,011,497,696 possible user-product combinations, leading to a completion of approximately **3.91 * 10^-4 %**. This scarcity poses challenges and dictates the type of recommendation algorithms that can be

## Results
We compared different models and found that the optimized Matrix Factorization model-based collaborative filtering (svd_optimized) stood out as a strong performer, offering accurate and personalized recommendations.

Here are the results obtained from various recommendation models used in this project:

**Model Name: User-user similarity-based collaborative filtering: knn_user**
- RMSE: 1.0250
- Precision:  0.86
- Recall:  0.783
- F_1 score:  0.82

**Model Name: knn_user_optimized**
- RMSE: 0.9621
- Precision:  0.852
- Recall:  0.809
- F_1 score:  0.83

**Model Name:  Item-item similarity-based collaborative filtering: knn_item**
- RMSE: 1.0232
- Precision:  0.835
- Recall:  0.758
- F_1 score:  0.795

**Model Name: knn_item_optimized**
- RMSE: 0.9703
- Precision:  0.834
- Recall:  0.799
- F_1 score:  0.816

**Model Name: Model-based (matrix factorization) collaborative filtering: svd**
- RMSE: 0.8989
- Precision:  0.86
- Recall:  0.797
- F_1 score:  0.827

**Model Name: svd_optimized**
- RMSE: 0.8899
- Precision:  0.862
- Recall:  0.796
- F_1 score:  0.828


## Licensing, Authors, and Acknowledgements

Author: Syed Raif Rizvi

Acknowledgements: The dataset and scenario used in this project was provided as part of a problem assignment during the [MIT IDSS Certification](https://www.mygreatlearning.com/mit-data-science-and-machine-learning-program?gl_campaign=Eportfolio&gl_source=Linkedin&utm_source=eportfolio).
