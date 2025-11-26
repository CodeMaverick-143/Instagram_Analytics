# Instagram Post Analytics and Engagement Prediction

This project analyzes a dataset of 30,000 Instagram posts collected over the last 12 months. The dataset contains detailed engagement metrics including likes, comments, shares, saves, reach, impressions, hashtags used, caption length, followers gained, and content type. The goal of this project is to study posting behavior, identify high-performing patterns, and build machine learning models to predict engagement and classify content performance.

---

## Project Objectives

1. Analyze Instagram content performance over the last 365 days.
2. Identify meaningful patterns affecting reach, engagement, and follower growth.
3. Study media types such as Reels, Photos, Videos, and Carousels comparatively.
4. Evaluate the role of traffic sources such as Explore, Reels feed, Home feed, Profile, and Hashtags.
5. Build machine learning models to:

   * Predict engagement rate of posts
   * Classify high vs low performing content
6. Generate actionable insights for creators and growth strategists.

---

## Dataset Features

| Column           | Description                        |
| ---------------- | ---------------------------------- |
| Post_ID          | Unique post identifier             |
| Upload_Date      | Posting date within the last year  |
| Media_Type       | Photo, Video, Reel, or Carousel    |
| Likes            | Total likes on the post            |
| Comments         | Number of comments                 |
| Shares           | Total shares                       |
| Saves            | Number of users who saved the post |
| Reach            | Unique accounts reached            |
| Impressions      | Total views including repeats      |
| Caption_Length   | Caption character count            |
| Hashtags_Count   | Number of hashtags used            |
| Followers_Gained | Followers obtained from this post  |
| Traffic_Source   | Source of impressions              |
| Engagement_Rate  | Engagement based on impressions    |

---

## Work Flow

### Stage 1: Data Preparation

* Load the dataset using pandas
* Convert date column into datetime format
* Extract month, weekday, and post age
* Handle missing values
* Encode categorical variables using one-hot encoding

### Stage 2: Exploratory Data Analysis

* Distribution of likes, reach, impressions, saves, engagement rate
* Performance comparison between media types
* Engagement influence of hashtags and caption length
* Traffic source based content reach comparison
* Correlation matrix and insight extraction

### Stage 3: Machine Learning Models

#### Engagement Rate Regression

* Random Forest Regressor used to estimate engagement rate
* Metrics evaluated:

  * Mean Absolute Error (MAE)
  * R-squared (R2)

#### High vs Low Performance Classification

* Engagement threshold defined using median split
* Random Forest Classifier modeled for binary classification
* Evaluation metrics:

  * Accuracy
  * Precision
  * Recall
  * Confusion Matrix

---

## Key Insights to be Derived

After executing the notebook, the following conclusions are drawn:

1. Most effective content formats for engagement and reach
2. Optimal caption length and hashtag count ranges
3. Traffic source performance and discoverability patterns
4. Contribution of saves, reach, impressions, and followers gained to engagement
5. Most important features from model explainability
6. Ability to predict high-performing content before posting

---

## Results Section (Fill after training)

Replace values after running notebook.

| Model                           | Result |
| ------------------------------- | ------ |
| Regression MAE                  |        |
| Regression R2                   |        |
| Classification Accuracy         |        |
| Classification Precision/Recall |        |

Feature Importance Summary:

* Top driving factors include:

  * Saves
  * Reach
  * Media Type
  * Traffic Source
  * Hashtag count
  * Caption length

---

## Final Outcome

This project provides a complete pipeline to understand Instagram content performance and forecast engagement. The insights generated can be used to guide creators, marketers, and influencers to optimize posting strategies. The machine learning models built are capable of predicting performance trends and identifying high-impact factors responsible for growth.
