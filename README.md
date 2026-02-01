# House Price Prediction — Regression

This repository contains my solution notebook for the **House Price Prediction** competition conducted as part of the **IIT Madras BS in Data Science & Applications** program.

The task was to predict house prices for different districts using demographic and housing-related features.

---

## Task Summary
- **Problem type:** Regression  
- **Target variable:** `TargetPrice`  
- **Evaluation metric:** RMSE (Root Mean Squared Error)  

`TargetPrice` represents the median house value in units of **$100,000**  
(e.g., `2.35` → `$235,000`).

---

## Dataset
The dataset provided for the competition is based on the California Housing data and includes:
- Noisy features  
- Missing values (especially in `PropertyAge`)  
- Obfuscated column names  

### Files used
- `estate_train.csv` – training data with target values  
- `estate_test.csv` – test data without target values  
- `estate_sample_submission.csv` – submission format  

---

## What I Did
- Cleaned and preprocessed the data  
- Handled missing values in the dataset  
- Scaled numerical features where required  
- Performed basic exploratory data analysis  
- Trained regression models  
- Evaluated performance using RMSE  
- Generated predictions for the final submission  

---

## Challenges Faced
- Features with very different scales  
- Missing values in key columns  
- Presence of outliers in some districts  
- Noise added to simulate real-world data  

---

## Submission
Predictions were submitted in the following format:

```csv
PropertyID,TargetPrice
abc123,2.45
xyz789,1.98
