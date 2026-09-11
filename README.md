# Predicting Waze User Churn
## Overview
The goal of this project was to develop a churn prediction model that will help prevent churn, improve user retention, and grow Waze’s business. This project utilized different Waze users were classification of churned/retained has been made. The final XGBoost model performed with 80% accuracy and 41% precision determining what features were most important in separating churned from retained users. Based on the model, number of days after onboarding, km per hour, total navigations to favorite places, ration between last month sessions to total sessions and drives duration in minutes were the most influential in determining a churned user versus a retained .

## Business Understanding
High retention rates indicate satisfied users who repeatedly use the Waze app over time. An accurate model can help identify specific factors that contribute to churn. These insights will help Waze leadership optimize the company’s retention strategy, enhance user experience, and make data-driven decisions about product development. By answering questions such as: Who are the users most likely to churn? Why do they churn? When do users churn? Waze can proactively engage these users with special offers to try and retain them. Otherwise, Waze may simply lose these users without knowing why. 

## Data Understanding
This project uses a dataset called waze_dataset.csv. It contains synthetic data created for this project in partnership of Google advanced data analytics certificate program with Waze. The dataset contains unique 14,999 user and 13 feature for each one. The features included information on number of last month sessions and drives, days since a user signed up, user device type, total session, navigations to favorite places and more features about their driving behavoir. Approximately 18% of the users in this dataset churned, compared to 82% whom retained. <br> <br>  <img width="259" height="231" alt="download" src="https://github.com/user-attachments/assets/0b2d2dce-19bf-4dca-832a-60f88d6f3c7c" />

In connection to this, new features was engineered. Multiple redundant columns were dropped and encoded into the proper data type.  

## Modeling and Evaluation 
An XGBoost model comprising 200 decision trees was used to determine feature importance in user classification as a churned or not. The below plot shows that number of days after onbarding, km driven per hour and total navigations to the favorite place were the top 3 most important factors in determining a churn status. The overall model performance after testing was  80% accuracy and 24.4% f1-score. <br> <br>
<img width="1146" height="664" alt="Screenshot from 2026-09-10 19-45-13" src="https://github.com/user-attachments/assets/7039272f-e3e1-418f-996e-a7826f936238" />



## Conclusion
It is not recommended to use the current model for churn prediction, because it yielded many false negative errors where it indicated users who will churn as retained. However, the model will be of huge benefit for guiding future exploratory analysis efforts. Furthermore, data could be joined that need to balance the classes in the target variable to revel more about churn customer behavior. Also more feature engineering could be done since it is one of the easiest and fastest ways to improve model performance.
