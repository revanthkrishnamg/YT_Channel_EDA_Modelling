# YouTube Channel Engagement Optimization Project

## Overview
This project analyzes my YouTube channel to optimize viewer engagement. Utilizing the YouTube API, it systematically evaluates video views and interactions. Various predictive models are built and compared to accurately classify video engagement levels as either high or low. The project harnesses machine learning techniques and data-driven insights to identify patterns and factors contributing to higher engagement.

## Repository Content
- **1_Data_Collection.ipynb**: Gathers data from my YouTube Channel using the YouTube API.
- **2_Data_Preparation_EDA.ipynb**: Data cleaning, preprocessing, and exploratory data analysis.
- **3_Classification_Modelling.ipynb**: Develops a classification model to predict high or low video engagement.

## Data Collection
Using the YouTube API, channel and video statistics were collected, including subscriber counts, total views, likes, comments, and detailed video metrics. Viewer comments were analyzed for sentiment to provide deeper insights into audience preferences.

## Data Preparation
- Missing descriptions were replaced with "Empty."
- Non-numeric 'comment_count' values were converted to numeric.
- Video durations were converted from ISO 8601 format to seconds.
- Duplicates and outliers were removed to ensure data integrity.
- Categorical data like 'category_id' and 'video_status' were refined.

## New Features for Analysis
- **Time of Upload**: Extracted hour, day, month, and year; identified weekends.
- **Video Length Category**: Categorized videos into short (0-60s), medium (60-300s), and long (300s+).
- **Engagement Ratios**: Calculated likes-to-views, comments-to-views, and likes-to-comments ratios.
- **Net Subscriber Gain per Video**: Computed net subscriber gains for each video.
- **Engagement Score (0-100)**: Created a weighted score based on views, likes, and comments.
- **Engagement Category**: Classified videos into 'High' or 'Low' based on engagement scores.

## Exploratory Data Analysis (EDA)
- Analyzed engagement score distribution, time series, and video length categories.
- Performed sentiment analysis on viewer comments.
- Identified optimal days and times for posting to maximize engagement.

## Model Building
Models including Logistic Regression, KNN, Decision Tree, Random Forest, and AdaBoost were built and compared. AdaBoost, after hyper-parameter tuning, was selected as the best model based on its performance metrics.

## Model Evaluation
The AdaBoost model demonstrated high accuracy and balanced classification abilities. The ROC curve indicated that the model generalized well without overfitting.

## Recommendations
- Optimize video length for increased engagement.
- Utilize high-impact keywords identified in the analysis.
- Schedule uploads during peak engagement times.
- Focus on producing high-definition content.

## Conclusion
This project identifies key drivers of engagement on my YouTube channel. The insights and models developed can guide strategic content planning to improve channel performance.
