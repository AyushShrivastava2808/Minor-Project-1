# 🚗 Car Price Prediction using Machine Learning

## 📌 Problem Statement
The automobile industry generates a large amount of data related to vehicle specifications and pricing. Determining the appropriate price of a car is important for both buyers and sellers. Car prices depend on several factors such as engine size, horsepower, fuel type, vehicle dimensions, mileage, and other technical specifications.

The objective of this project is to develop a machine learning model that can predict the price of a car based on its features. This prediction can help customers estimate the value of a vehicle and assist businesses in making data-driven pricing decisions.

---

## 🎯 Project Objectives
- Analyze a real-world car pricing dataset.
- Perform data preprocessing and exploratory data analysis (EDA).
- Train supervised machine learning models for price prediction.
- Compare the performance of different algorithms.
- Select the most accurate model for car price prediction.

---

## 📂 Dataset Description
- **Total Records**: 205  
- **Total Features**: 26  
- **Target Variable**: `price`

### Features include:
- Fuel Type  
- Aspiration  
- Number of Doors  
- Car Body Type  
- Drive Wheel Type  
- Wheelbase, Car Length, Car Width, Car Height  
- Curb Weight  
- Engine Type, Number of Cylinders, Engine Size, Horsepower  
- Fuel System  
- Mileage (City MPG and Highway MPG)  

---

## 🛠️ Data Preprocessing
1. **Missing Values**: Checked using `df.isnull().sum()` → No missing values found.  
2. **Duplicate Records**: Removed using `df.duplicated().sum()`.  
3. **Feature Removal**: Dropped `car_ID` (unique identifier).  
4. **Feature Encoding**: Applied Label Encoding to categorical columns.  
5. **Feature Scaling**: StandardScaler applied for Linear Regression model.  

---

## 📊 Exploratory Data Analysis (EDA)
- **Car Price Distribution**:  
  - Most cars fall within lower and medium price ranges.  
  - A few expensive cars act as outliers.  
  - Distribution is slightly right-skewed.  

- **Correlation Analysis**:  
  - Engine Size, Horsepower, and Curb Weight strongly positively correlated with price.  
  - Highway MPG and City MPG negatively correlated with price.  

---

## 🤖 Machine Learning Models
### 1. Linear Regression
- ✅ Simple, interpretable, fast training.  
- ❌ Assumes linearity, struggles with complex patterns.  

### 2. Random Forest Regressor
- ✅ Handles non-linear relationships, reduces overfitting, higher accuracy.  
- Selected as the **final model** due to better performance.  

---

## ⚙️ Training Process
Workflow followed:
1. Load Dataset  
2. Data Cleaning  
3. Data Encoding  
4. Feature Scaling  
5. Train-Test Split (80:20)  
6. Model Training  
7. Prediction  
8. Evaluation  

---

## 📈 Model Evaluation
Metrics used:
- **MAE** (Mean Absolute Error)  
- **MSE** (Mean Squared Error)  
- **RMSE** (Root Mean Squared Error)  
- **R² Score**

---

**Analysis**:  
Random Forest achieved higher R² and lower error values compared to Linear Regression, making it the best model for car price prediction.

---

## 📌 Conclusion
- Random Forest Regressor is the most effective model for predicting car prices.  
- Engine Size, Horsepower, and Curb Weight are the most influential features.  
- This project demonstrates how machine learning can assist in data-driven pricing decisions in the automobile industry.  

---

## 🚀 Future Work
- Use larger datasets for better generalization.  
- Try advanced models like Gradient Boosting, XGBoost, or Neural Networks.  
- Deploy the model as a web app using **Streamlit** or **Flask**.  

---

## 📝 Author
Developed by **Ayush Shrivastava**  
B.Tech CS (2024–2028)  

