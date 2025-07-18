# ⚡ EV Adoption Forecasting

This project focuses on predicting the future adoption of Electric Vehicles (EVs) using historical vehicle registration data from Washington State. It uses machine learning techniques to help urban planners and policymakers anticipate the growing demand for EV infrastructure—especially charging stations.


## 📌 Objective

To build a regression model that accurately forecasts future EV adoption trends using historical data, helping in sustainable infrastructure planning.

---

## 📊 Dataset Overview

- **Source:** Washington State Department of Licensing (2017–2024)
- **Key Features:**
  - `Date` (Monthly registration date)
  - `County` and `State`
  - `Vehicle Primary Use` (Passenger or Truck)
  - `Battery Electric Vehicles (BEVs)`
  - `Plug-in Hybrid Electric Vehicles (PHEVs)`
  - `Electric Vehicle (EV) Total`
  - `Non-Electric Vehicle Total`
  - `Percent Electric Vehicles`

---

## ⚙️ Technologies Used

- Python 🐍
- Pandas & NumPy – data handling
- Seaborn & Matplotlib – data visualization
- Scikit-learn – model training, tuning, evaluation
- Joblib – model saving and loading

---

## 🔍 Key Steps

1. **Data Cleaning:**
   - Convert dates to datetime format
   - Remove or fill missing values
   - Handle and cap outliers using the IQR method

2. **Feature Engineering:**
   - Time-based features (e.g., year, month)
   - Encoding categorical columns

3. **Model Building:**
   - Random Forest Regressor
   - Hyperparameter tuning with `RandomizedSearchCV`

4. **Evaluation:**
   - Metrics: MAE, MSE, R² Score
   - Visualization of predictions vs actual data

---

## 🧠 Results

- Accurate predictions of EV growth over time
- Identified key trends per county and vehicle type
- Outlier handling improved model robustness

---

## 💾 How to Run

1. Clone the repository  
   ```bash
   git clone https://github.com/yourusername/EV-Adoption-Forecasting.git
   cd EV-Adoption-Forecasting
