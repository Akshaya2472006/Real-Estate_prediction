# 🏠 Real Estate Price Prediction

## 📌 Project Overview
This project analyzes the **King County Housing Dataset** to uncover insights into property features and their impact on house prices.  
It builds a **Linear Regression model** to predict housing prices based on features such as square footage, bedrooms, bathrooms, and location.  

---

## 📑 Table of Contents
- Dataset Overview  
- Exploratory Data Analysis (EDA)  
- Feature Engineering  
- Model Building  
- Evaluation Metrics  
- Visualizations  
- Key Insights  
- How to Run  
- Author  

---

## 📂 Dataset Overview
**File:** `kc_house_data.csv`

**Columns:**
- `id`, `date`, `price` (target variable)  
- `bedrooms`, `bathrooms`, `floors`  
- `sqft_living`, `sqft_lot`, `sqft_above`, `sqft_basement`  
- `waterfront`, `view`, `condition`, `grade`  
- `yr_built`, `yr_renovated`, `zipcode`, `lat`, `long`  
- `sqft_living15`, `sqft_lot15`  

---

## 🔍 Exploratory Data Analysis (EDA)
- Distribution of house prices  
- Correlation between features and price  
- Impact of square footage on price  
- Regional distribution of house prices  

---

## 🛠 Feature Engineering
- Converted `date` into **year, month, day** features  
- Selected key numerical features (`sqft_living`, `bedrooms`, `bathrooms`)  
- Applied preprocessing pipelines:  
  - **Numerical:** StandardScaler  
  - **Categorical:** OneHotEncoder (for `zipcode`)  

---

## 🤖 Model Building
**Algorithm:** Linear Regression  

**Steps:**
- Split dataset into training and testing sets  
- Fit the model on training data  
- Evaluate predictions on test data  

---

## 📸 Visualizations

### 1. Price Distribution
![Price Distribution](images/price_distribution.png)

### 2. Correlation Heatmap
![Correlation Heatmap](images/correlation_heatmap.png)

### 3. Sqft Living vs Price
![Sqft vs Price](images/sqft_vs_price.png)

### 4. Actual vs Predicted Prices
![Actual vs Predicted](images/actual_vs_predicted.png)

### 5. Residuals Distribution
![Residuals](images/residuals.png)

---

## 📈 Evaluation Metrics
- **R² Score:** ~0.65  
- **MAE:** 125,000 (approx.)  
- **RMSE:** 180,000 (approx.)  

---

## 🧩 Key Insights
- **Sqft Living** is the most influential feature in predicting price.  
- Houses with higher grades and better condition tend to have higher prices.  
- Waterfront properties show significantly higher average prices.  
- The model performs moderately well, but advanced models (Random Forest, XGBoost) could improve accuracy.  

---

## ▶️ How to Run
1. Clone the repository:  
   ```bash
   git clone https://github.com/Akshaya2472006/Real-Estate_prediction.git
