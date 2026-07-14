# NBA MVP Predictor 2026-27

**Predicting the 2026-27 NBA Most Valuable Player using Machine Learning**

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![XGBoost](https://img.shields.io/badge/XGBoost-35495E?style=for-the-badge&logo=xgboost&logoColor=white)

---

## 📋 Project Overview

This project predicts the top MVP candidates for the 2026-27 NBA season using player performance data from the 2026 season. I used XGBoost Regression with advanced basketball metrics to estimate player impact.

**Best Model Performance:**
- **XGBoost Regressor** → **R² Score: 0.9749**

---

## 📊 Model Results

| Metric                        | Value     |
|-------------------------------|-----------|
| R² Score (Variance Explained) | **0.9749** |
| Mean Absolute Error (MAE)     | 18.33     |

---

## 🏆 Top 10 Predicted MVP Candidates (2026-27)

1. **Shai Gilgeous-Alexander (OKC)**
2. **Luka Dončić (LAL)**
3. **Victor Wembanyama (SAS)**
4. **Kevin Durant (HOU)**
5. **Nikola Jokić (DEN)**
6. **Karl-Anthony Towns (NYK)**
7. **Scottie Barnes (TOR)**
8. **Tyrese Maxey (PHI)**
9. **Amen Thompson (HOU)**
10. **Jamal Murray (DEN)**

---

## 🔍 Key Insights

- **Shai Gilgeous-Alexander** and **Luka Dončić** emerge as the top frontrunners.
- Playing time (MIN) and scoring efficiency (PPG) are the most important factors for MVP prediction.
- Advanced metrics like True Shooting Percentage and Usage Rate add significant value.

**Feature Engineering:**
- Per-game stats (PPG, RPG, APG)
- Efficiency metrics (TS%, Usage Rate)
- Availability filter (min 50 games)

---

## 🗂️ Project Structure
nba-mvp-predictor/
├── notebooks/
│   └── NBA_MVP_Prediction.ipynb
├── README.md
├── requirements.txt
└── .gitignore


---

## 🛠️ How to Run

1. Clone the repository
   ```bash
   git clone https://github.com/adas1496/nba-mvp-predictor.git
   cd nba-mvp-predictor

2. Install dependencies
pip install -r requirements.txt

3. Run the notebook
Open notebooks/NBA_MVP_Prediction.ipynb

👤 Author
Aman Das
Aspiring AI/ML Engineer

 ⭐**Show Your Support**
 
 If you found this project useful, please give it a star!⭐ 


  
