# Predicting Waze User Churn
## Overview
The goal of this project was to develop a churn prediction model that will help prevent churn, improve user retention, and grow Waze’s business. This project utilized different Waze users were classification of churned/retained has been made. The final XGBoost model performed with 80% accuracy and 41% precision determining what features were most important in separating churned from retained users. Based on the model, number of days after onboarding, km per hour, total navigations to favorite places, ration between last month sessions to total sessions and drives durations in minutes were the most influential in determining a churned user versus a retained .

## Business Understanding
TikTok users have the ability to report videos and comments that contain user claims. These reports identify content that needs to be reviewed by moderators. This process generates a large number of user reports that are difficult to address quickly. With a successful prediction model, TikTok can reduce the backlog of user reports and prioritize them more efficiently.

## Data Understanding
This project uses a dataset called tiktok_dataset.csv. It contains synthetic data created for this project in partnership of Google advanced data analytics certificate program with TikTok. The dataset contains unique 19,383 video and 12 features for each one. The features included information on video claim status, duration, transcription text, and counts of different interactions. Also included author verification and ban status. The bar chart below shows the breakdown of how many claim videos versus opinion videos that exist in the data set. <br> <br>
<img width="1023" height="630" alt="Sheet 2" src="https://github.com/user-attachments/assets/4ed71ce0-19f4-48b5-b901-896be6e64034" />
In connection to this, a feature was engineered to represent the transcript text length. Multiple redundant columns were dropped and encoded into the proper data type.  

## Modeling and Evaluation 
A random forest model comprising 75 decision trees was used to determine feature importance in video classification as a claim or not. The below plot shows that video views, likes, and downloads were the Top 3 most important factors in determining a claim video. The overall model performed with same scores after testing, nearly 100% accuracy and 99% recall. <br> <br>
<img width="777" height="879" alt="image" src="https://github.com/user-attachments/assets/c5298422-362b-431e-b4d8-5bdb7f3b66b7" />

## Conclusion
it is highly recommended to start using the model in a trial because it shows good measures and any helpful feedback would be of high benefit for further improvement. Getting the number of reports done by users on each claim classified video could be very useful where we can arrange claim videos by number of reports in descending order and review them manually. 
