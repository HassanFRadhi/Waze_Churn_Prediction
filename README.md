# Predicting Waze User Churn
## Overview
The goal of this project was to develop a churn prediction model that will help prevent churn, improve user retention, and grow Waze’s business. This project utilized different Waze users were classification of churned/retained has been made. The final XGBoost model performed with 80% accuracy and 41% precision determining what features were most important in separating churned from retained users. Based on the model, number of days after onboarding, km per hour, total navigations to favorite places, ration between last month sessions to total sessions and drives duration in minutes were the most influential in determining a churned user versus a retained .

## Business Understanding
High retention rates indicate satisfied users who repeatedly use the Waze app over time. An accurate model can help identify specific factors that contribute to churn. These insights will help Waze leadership optimize the company’s retention strategy, enhance user experience, and make data-driven decisions about product development. By answering questions such as: Who are the users most likely to churn? Why do they churn? When do users churn? Waze can proactively engage these users with special offers to try and retain them. Otherwise, Waze may simply lose these users without knowing why. 

## Data Understanding
This project uses a dataset called waze_dataset.csv. It contains synthetic data created for this project in partnership of Google advanced data analytics certificate program with Waze. The dataset contains unique 14,999 user and 13 feature for each one. The features included information on number of last month sessions and drives, days since a user signed up, user device type, total session, navigations to favorite places and more features about their driving behavoir. Approximately 18% of the users in this dataset churned, compared to 82% whom retained.
In connection to this, new features was engineered. Multiple redundant columns were dropped and encoded into the proper data type.  

## Modeling and Evaluation 
A random forest model comprising 75 decision trees was used to determine feature importance in video classification as a claim or not. The below plot shows that video views, likes, and downloads were the Top 3 most important factors in determining a claim video. The overall model performed with same scores after testing, nearly 100% accuracy and 99% recall. <br> <br>
<img width="777" height="879" alt="image" src="https://github.com/user-attachments/assets/c5298422-362b-431e-b4d8-5bdb7f3b66b7" />

## Conclusion
it is highly recommended to start using the model in a trial because it shows good measures and any helpful feedback would be of high benefit for further improvement. Getting the number of reports done by users on each claim classified video could be very useful where we can arrange claim videos by number of reports in descending order and review them manually. 
