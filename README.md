# Udacity - Data Scientist Capstone Project: Sparkify - Customer Churn Prediction Model

## Table of Contents
1. Description
2. Dependencies
3. Executing Program
4. Defined Features and Models
5. Author
6. License
7. Acknowledgement

### 1. Description

Like Spotify and fizy, Sparkify is music streaming application. Udacity provides datasets of Sparkify user log transactions. Mini dataset (128MB) and the full dataset (12GB) are also available.

In this project, I completed steps (methodology) below to implement model predicting potential users who will churn. Then, Sparkify can identify users who are likely cancel your service membership, then Sparkify can send marketing offers or campaign to them to preventing churn and revenue leakage. I also used mini dataset in Jupyter notebook. 

1. Load and Clean Dataset
2. Exploratory Data Analysis and Defining Churn Label 
3. Feature Engineering
4. Test Models and Determine Best Model with tuning parameters.

Medium blog post is also written to explain details of these steps. 

Medium Link: https://dev.to/ankit1797/sparkify-digital-music-service-customer-churn-analysis-prediction-14de

### 2. Dependencies

Python 3.5+
Python libraries: pandas, numpy, matplotlib.pyplot, seaborn, time, date time
Pyspark 2.4
Pyspark.ml
Pyspark.sql

Dataset: “mini_sparkify_event_data.json” is the user transactional log data that provided by Udacity before starting project.

Models: Logistic Regression, Random Forest, Gradient Boosted Trees

### 3.Executing Program
File structure of project is showed below. Jupyter notebook can be executed. 

|- Sparkify.ipynb  # Notebook importing related packages, cleaning, processing the data, data analysis and ml pipeline (models).
|- mini_sparkify_event_data.json  # Sparkify user transactional log data provided by Udacity 
|- README.md # ReadME file


### 4. Defined Features and Models:

Churn is defined as Cancellation Confirmation events in mini_sparkify_event_data.json data.

Following 10 features are defined to build models
1. Average listened songs per session
2. Listened total songs by users
3. Number of Add Friend transactions
4. Number of Add Playlist transactions
5. Number of Thumbs Down transactions
6. Number of Thumbs Up transactions
7. Register duration (days) - between last event date of user and registration date.
8. Length of listen time 
9. Gender
10. Account level


Random Forest Model performs the best on the dataset provided which provides a F1 score of 0.949.


### 5. Author
Ankit Patel - Udacity Student in Data Science Nanodegree

### 6. License
Udacity 

### 7. Acknowledgement
Udacity for providing great online lessons in Data Science Nanodegree Program