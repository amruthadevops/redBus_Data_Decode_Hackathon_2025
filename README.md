
# 🚌 redBus Data Decode Hackathon 2025 – Seat Demand Forecasting (🏆 8th Place Winner)

Forecasting future bus seat demand at a route level — 15 days in advance — using real-world booking, issue, and search data.



## 🏆 Hackathon Achievement

This project secured **8th place out of hundreds of participants** in the prestigious **redBus Data Decode Hackathon 2025**.

---


## 📌 Problem Statement

Given historical booking data (`seats_booked`, `date_of_journey`, `date_of_issue`, and search logs), forecast the **number of seats likely to be booked** for each route, exactly **15 days before the journey date**.

The goal was to minimize **Root Mean Square Error (RMSE)** between predicted and actual bookings.

## 🚀 Solution Overview

1. **Feature Engineering**:
   - Created date-based lag/lead features
   - Extracted weekday, weekend, festival/holiday flags
   - Captured trend dynamics using rolling windows and decay functions

2. **Modeling**:
   - Implemented ensemble of **XGBoost** and **LightGBM**
   - Used **custom objective tuning** to optimize for RMSE
   - Applied **early stopping and CV-based ensembling**

3. **Evaluation**:
   - Achieved RMSE ~550 on local CV
   - Leaderboard RMSE: **534**



## 📊 Technical Stack

| Area                | Tools & Libraries                                 |
|---------------------|---------------------------------------------------|
| Language            | Python                                             |
| Data Manipulation   | Pandas, NumPy                                      |
| Visualization       | Seaborn, Matplotlib, Plotly                        |
| Machine Learning    | XGBoost, LightGBM, Scikit-learn                    |
| Evaluation         | RMES, Feature Importance Plot,    |
| Feature Engineering | Sklearn , Holidays, Datetime manipulation                          |
| Final Submission    | CSV with forecasts + notebook walkthrough         |


## ⚙️ Reproducibility


```bash
1. Clone the repo:
  
   git clone https://github.com/amruthadevops/redBus_Data_Decode_Hackathon_2025.git
   cd redBus_Data_Decode_Hackathon_2025

2. Install dependencies:
    pip install -r requirements.txt

3. Open the notebook:
    jupyter notebook notebooks/Final_Submission.ipynb

```
    
## 🧠 Skills Demonstrated
- 🧹 Data Cleaning and Preprocessing

- 📐 Feature Engineering for Temporal Forecasting

- 📈 Tree-based Model Optimization (XGBoost, LightGBM)

- 🎯 RMSE-focused Model Evaluation

- 💡 Real-world Business Understanding (supply/demand balance)
## ⚡ Key Highlights

#### 🎯 Rich Feature Engineering:

    - Calendar features (weekday, month, festival/wedding cues)

    - National holiday signals and long weekend detection

    - Region/tier classification and composite route encoding

    - Rolling stats and trend slopes from historical booking/search logs

    - High-impact interaction features including demand skew ratios and search densities

#### 📈 Advanced Modeling Workflow:

    - LightGBM with early stopping and hyperparameter tuning

    - Ridge-based bias correction on temporal attributes

    - Time-based train/validation split to reduce leakage

#### 🧪 Performance Benchmark:

    - Final validation RMSE: 532

    - Feature importance visualized using gain metrics

#### 🔄 Post-processing Strategy:

    - Confidence boosting for high-frequency routes

    - Clipped and rounded predictions for realistic output formatting
## 🔗 Acknowledgments

 - Thanks to redBus and Analytics Vidhya for organizing the challenge and providing valuable data.


## ✨ Professional Snapshot
``` 
"Engineered a predictive seat demand model by fusing cultural, transactional, and temporal features. Delivered high-performance predictions via LightGBM, bias correction, and dynamic post-processing. Demonstrated full-cycle modeling, leaderboard tuning, and explainability."
```
