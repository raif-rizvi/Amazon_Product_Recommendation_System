# Amazon_Product_Recommendation_System
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
Scenario : As a Data Science Manager at Amazon, I was tasked to build a recommendation system that could enhance the user experience by suggesting products based on their previous ratings. 

## File Descriptions
The repository contains the following file:
- `Amazon_Product_Recommendation_System.ipynb`: This is the Google Colab Notebook where all the work is done, which includes data loading, preprocessing, exploratory data analysis, model building, and evaluation.

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

This project is licensed under the MIT License - see the LICENSE file for details.

Author: Syed Raif Rizvi

Acknowledgements: The dataset used in this project was provided as part of a problem assignment during the [MIT IDSS Certification](https://www.mygreatlearning.com/mit-data-science-and-machine-learning-program?gl_campaign=Eportfolio&gl_source=Linkedin&utm_source=eportfolio).
