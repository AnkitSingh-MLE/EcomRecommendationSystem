# EcomRecommendationSystem
Recommendation system using KNN
E-Commerce Purchase Analysis and Recommendation System

Project Overview

This project focuses on analyzing customer purchase behavior in an e-commerce setting and building a recommendation system using the k-Nearest Neighbors (KNN) algorithm. The dataset used contains transaction details, including customer ID, product category, payment method, time spent on the site, and other relevant features. The analysis includes feature engineering, exploratory data analysis (EDA), feature importance analysis using Random Forest, and building a recommendation system based on user similarity.

Dataset

The dataset consists of 24,999 records with the following features:

date: Transaction date

customer_id: Unique identifier for each customer

product_category: Category of the purchased product

payment_method: Payment method used (credit, PayPal, etc.)

value [USD]: Transaction amount in USD

time_on_site [Minutes]: Time spent on the site per transaction

clicks_in_site: Number of clicks made during the session

Unnamed: 7: An irrelevant column that was removed

Project Steps

1. Data Preprocessing

Loaded the dataset and checked for missing values.

Converted the date column to a datetime format and extracted weekday, hour, and month features.

Computed total spending per customer and average transaction value.

Normalized numerical features using StandardScaler.

Encoded categorical variables using LabelEncoder.

2. Exploratory Data Analysis (EDA)

Visualized the distribution of purchases by hour of the day.

Analyzed total spending and average transaction value distributions.

Computed the feature correlation matrix using a heatmap.

3. Feature Importance Analysis

Used a Random Forest Regressor to determine feature importance in predicting purchase value.

Identified key influencing factors such as total_spent, avg_transaction_value, and clicks_in_site.

4. Recommendation System using k-Nearest Neighbors (KNN)

User-Based Similarity

Built a recommendation model using KNN with cosine similarity.

Identified the top 5 similar users based on purchase behavior.

User-Item Interaction Matrix

Created a user-item matrix based on payment_method and avg_transaction_value.

Applied KNN to find users with similar transaction patterns.

Results

Successfully analyzed customer purchase behavior and identified key influencing factors.

Built a recommendation system using KNN that finds similar users based on transaction data.

Technologies Used

Programming Language: Python

Libraries: pandas, numpy, matplotlib, seaborn, scikit-learn

