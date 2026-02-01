# 🏠 House Price Prediction — IIT Madras Competition

## 📌 Overview
This project is part of the **House Price Prediction Competition conducted by IIT Madras**.  
The objective is to build a **regression model** that accurately predicts house prices for different districts using demographic and structural features.

The dataset is inspired by the California Housing dataset and modified to reflect **real-world data challenges**, including noise, missing values, and feature obfuscation.

---

## 🎯 Problem Statement
Predict the continuous variable **`TargetPrice`**, which represents the **median house value** of a district.

- Unit: **$100,000**
- Example: `2.35` → `$235,000`

---

## 📊 Evaluation Metric
Model performance is evaluated using **Root Mean Squared Error (RMSE)**:

\[
RMSE = \sqrt{\frac{1}{n}\sum_{i=1}^{n}(y_i - \hat{y}_i)^2}
\]

Lower RMSE indicates better prediction accuracy.

---

## 📁 Dataset Files

| File Name | Description |
|----------|-------------|
| `estate_train.csv` | Training dataset with features and target |
| `estate_test.csv` | Test dataset (features only) |
| `estate_sample_submission.csv` | Sample submission format |

---

## 🧾 Feature Description

| Feature | Description |
|-------|-------------|
| `PropertyID` | Unique identifier for each property cluster |
| `IncomeLevel` | Median income (in tens of thousands of dollars) |
| `PropertyAge` | Median age of houses *(contains missing values)* |
| `TotalRooms` | Average number of rooms per household |
| `TotalBedrooms` | Average number of bedrooms per household |
| `NeighborhoodPop` | Population of the district |
| `AvgOccupancy` | Average people per household |
| `RoomsPerHousehold` | Rooms-to-occupants ratio |
| `BedroomsRatio` | Bedrooms-to-rooms ratio |
| `TargetPrice` | Median house value (target variable) |

---

## ⚠️ Key Challenges
- **Feature scaling** due to large differences in magnitude  
- **Missing values** in `PropertyAge`  
- **Outliers** in room counts and occupancy  
- **Noise and obfuscated features** to simulate real-world data  

---

## 🛠️ Approach
Typical steps followed in this project:
1. Data cleaning and preprocessing  
2. Handling missing values  
3. Feature scaling  
4. Exploratory Data Analysis (EDA)  
5. Model training and evaluation  
6. Prediction on test data  
7. Submission file generation  

---

## 📤 Submission Format
The submission file must match the following format:

```csv
PropertyID,TargetPrice
abc123,2.45
xyz789,1.98
