🚗 Car Price Prediction Using Machine Learning
📌 Problem Statement
Accurate car price estimation is a critical challenge in the automobile industry. Buyers seek fair deals, while sellers aim to maximize returns. Car prices depend on multiple technical and design factors such as engine specifications, horsepower, fuel type, vehicle dimensions, mileage, and other attributes.

This project aims to build a machine learning model that predicts car prices based on vehicle features, enabling data-driven pricing decisions for customers and businesses.

🎯 Objectives
Perform data preprocessing and exploratory data analysis (EDA) on a real-world dataset.

Train and evaluate supervised machine learning models for price prediction.

Compare model performance using standard evaluation metrics.

Identify the most influential features affecting car prices.

Select the most accurate model for deployment.

📂 Dataset Overview
Records: 205

Features: 26

Target Variable: price

Key Features:
Fuel Type, Aspiration, Number of Doors

Car Body Type, Drive Wheel Type

Wheelbase, Car Length, Car Width, Car Height

Curb Weight

Engine Type, Cylinders, Engine Size, Horsepower

Fuel System

Mileage (City MPG, Highway MPG)

🛠️ Data Preprocessing
Missing Values: None detected.

Duplicates: Removed.

Feature Removal: Dropped car_ID (unique identifier).

Encoding: Applied Label Encoding to categorical features.

Scaling: StandardScaler applied for regression models requiring normalization.

📊 Exploratory Data Analysis (EDA)
Price Distribution:

Majority of cars fall in lower-to-mid price ranges.

Outliers exist in luxury/high-end cars.

Distribution is slightly right-skewed.

Correlation Insights:

Strong Positive: Engine Size, Horsepower, Curb Weight.

Negative: City MPG, Highway MPG.

🤖 Machine Learning Models
1. Linear Regression
✅ Fast, interpretable.

❌ Limited to linear relationships.

2. Random Forest Regressor
✅ Handles non-linear patterns, reduces overfitting.

✅ Achieved higher accuracy and robustness.

Selected as the final model.

⚙️ Workflow
Load Dataset

Clean Data

Encode Features

Scale Features

Train-Test Split (80:20)

Train Models

Predict Prices

Evaluate Performance

📈 Model Evaluation
Metrics used:

MAE (Mean Absolute Error)

MSE (Mean Squared Error)

RMSE (Root Mean Squared Error)

R² Score

Result:

Random Forest outperformed Linear Regression with higher R² and lower error values.

Key influential features: Engine Size, Horsepower, Curb Weight.

📌 Conclusion
Random Forest Regressor is the most effective model for car price prediction.

Engine specifications and weight are primary drivers of car pricing.

Demonstrates how ML can support data-driven decision-making in the automobile industry.

🚀 Future Enhancements
Use larger, more diverse datasets for improved generalization.

Experiment with advanced models (Gradient Boosting, XGBoost, Neural Networks).

Deploy as a web application using Streamlit or Flask for real-time predictions.

📝 Author
Ayush Shrivastava  
B.Tech Computer Science (2024–2028)
