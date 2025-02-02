# IndiGo Airline Passenger Referral Prediction
# Project Overview
This project aims to predict whether a passenger will recommend IndiGo Airlines based on various factors such as service quality, comfort, entertainment, and food & beverages. The classification model is trained on passenger reviews and ratings, using machine learning techniques to enhance customer satisfaction insights and business strategies.

# Dataset
* Total Rows: 131,895
* Total Columns: 17

# Key Features:
* Categorical: airline, author, customer_review, aircraft, traveller_type, cabin, route, date_flown, review_date, recommended
* Numerical: overall, seat_comfort, cabin_service, food_bev, entertainment, ground_service, value_for_money

# Handling Missing Values:
* Categorical: Replaced with mode values
* Numeric Ratings: Filled with median values
* Dates: Filled with the most frequent date

# Feature Engineering
* Extracted date-based features from review_date and date_flown
* One-hot encoding for traveller_type, cabin, and recommended
* Ordinal encoding for rating columns
* Principal Component Analysis (PCA) & Singular Value Decomposition (SVD) for dimensionality reduction

# Machine Learning Models
Three classification models were implemented:

# Model 1 - Random Forest Classifier
* Best Hyperparameters: { 'n_estimators': 100, 'min_samples_split': 3, 'min_samples_leaf': 1, 'max_depth': 20, 'bootstrap': True }
* Final Accuracy: 95.48%
# Model 2 - TBD
* Final Accuracy: 95.16%
# Model 3 - TBD
* Final Accuracy: 94.48%

# Evaluation Metrics
* Confusion Matrix
* Classification Report (Precision, Recall, F1-Score)
* Hyperparameter Tuning using RandomSearchCV

# Data Visualizations & Insights
* Airline vs Traveller Type vs Overall Rating (Heatmap)
* Overall Rating vs Seat Comfort (Scatter Plot)
* Correlation Matrix (Heatmap)
* Pair Plot for Key Features

# Conclusion & Business Impact
* Improving Seat Comfort & Cabin Service can increase positive recommendations
* Entertainment & Overall Rating have a strong correlation with passenger satisfaction
* Food & Beverage Quality plays a key role in the recommendation decision
