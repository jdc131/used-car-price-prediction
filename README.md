# Used Car Price Prediction 🚗

## Overview
This project focuses on predicting used car prices using machine learning techniques. The goal is to build models that can estimate a car’s price based on features such as engine size, mileage, make year, and ownership history.

This is a regression problem where the target variable is the car's selling price.

---

## Dataset
The dataset contains approximately 10,000 records of used cars and was obtained from Kaggle:

🔗 https://www.kaggle.com/datasets/therohithanand/used-car-price-prediction

### Key Features:
- Make Year  
- Mileage (km/l)  
- Engine Size (cc)  
- Fuel Type  
- Owner Count  
- Brand  
- Transmission  
- Color  
- Service History  
- Accidents Reported  
- Insurance Validity  

Target Variable:
- `price_usd`

---

## Data Preprocessing
- Loaded dataset using Pandas  
- Checked for missing values and data consistency  
- Converted categorical variables into numerical format  
- Split dataset into:
  - Features (X)
  - Target (y)
- Used an 80/20 train-test split  

---

## Exploratory Data Analysis (EDA)
The following visualizations were created:

- 📊 Distribution of Used Car Prices (Histogram)  
- 📈 Average Price by Make Year (Line Chart)  
- 📊 Average Price by Fuel Efficiency (Bar Chart)  
- 🔥 Correlation Matrix (Heatmap)  

### Key Insights:
- Newer cars generally have higher prices  
- Engine size has the strongest positive relationship with price  
- Owner count negatively affects price  
- Price distribution is slightly right-skewed  

---

## Models Used

### 1. Linear Regression
- Simple model assuming linear relationships  
- Easy to interpret  

### 2. Random Forest Regressor
- Ensemble model using multiple decision trees  
- Captures complex, non-linear relationships  

---

## Model Evaluation

| Model               | MAE     | RMSE    | R²    |
|--------------------|--------|--------|-------|
| Linear Regression  | 1005.38 | 1317.78 | 0.782 |
| Random Forest      | 959.83  | 1220.94 | 0.813 |

### Conclusion:
The Random Forest model performed better across all metrics, with:
- Lower error (MAE, RMSE)
- Higher R² score

---

## Feature Importance
The Random Forest model showed that:

1. Engine Size (most important)
2. Make Year
3. Mileage

Other features had smaller impact on predictions.

---

## Example Prediction
Sample Input:
- Make Year: 2015  
- Mileage: 12.09 km/l  
- Engine Size: 5000 cc  
- Fuel Type: Diesel  
- Owner Count: 1  

Prediction:
- Predicted Price: $12,354  
- Actual Price: $12,772  

This demonstrates that the model performs well on unseen data.

---

## Real-World Relevance
This project reflects how platforms like:
- Carvana  
- CarMax  
- Kelley Blue Book (KBB)  

use data-driven models to estimate car prices. These systems use similar features but often include additional data such as vehicle condition and market demand.

---

## Files Included
project.ipynb
used_car_price_dataset_extended.csv
presentation.pdf
report.pdf
README.md

## Author
Josh Custodio & Josh White 
University of West Florida  

---

## References
- Anand, R. (2025). Used car price prediction dataset. Kaggle.  
- Desai, M., & Deshpande, P. S. (2024). Predicting used car prices with supervised learning. SSRN.  
- Pal, N., Kumar, A., & Singh, R. (2017). Used car price prediction using random forest. arXiv.  
- Dhan, S. (2023). Used car price prediction. GitHub.  
