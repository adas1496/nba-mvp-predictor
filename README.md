# nba-mvp-predictor
Predicting the 2026-27 NBA MVP using XGBoost Regression, advanced analytics (True Shooting, Usage Rate), and data visualizations.  


**🏀 NBA MVP Predictor**

Predicting the top NBA MVP candidates for the 2026-27 season using Machine Learning.

**📋 Project Overview**
This project analyzes seasonal performance data for 582 NBA players from the 2026 season to predict the top MVP (Most Valuable Player) candidates for the upcoming 2026-27 season. The model is trained using XGBoost Regression to predict player overall efficiency (EFF), which serves as our proxy score for MVP voting impact.

Best Model Performance: XGBoost Regressor → R2 Score: 97.5%

**📊 Model Results**
The regressor was evaluated on an 80/20 train/test split, achieving exceptional precision in projecting player impact:

Metric                              Value
Mean Absolute Error (MAE)           18.33 
R² Score (Variance Explained)       0.9749  

**🏆 Top 5 Predicted Candidates**
Based on the final model outputs, these are the projected frontrunners:
1. Shai Gilgeous-Alexander (OKC) — 2183.81 Predicted Score
2. Luka Dončić (LAL) — 2144.64 Predicted Score
3. Nikola Jokić (DEN) — 2064.23 Predicted Score
4. Victor Wembanyama (SAS) — 2037.09 Predicted Score
5. Jalen Johnson (ATL) — 2028.32 Predicted Score

**🔍 Key Insights & Feature Engineering**
To measure player efficiency and workload accurately, we engineered advanced basketball metrics:

**True Shooting Percentage ($TS\%$):** Measures shooting efficiency by taking 2-pointers, 3-pointers, and free throws into account:
  
  $$TS\text{%} = \frac{\text{PTS}}{2 \times (\text{FGA} + 0.44 \times \text{FTA})} \times 100$$

  **Usage Rate ($USG\%$):** Estimates the percentage of team plays used by a player while they are on the court:
  
  $$\text{Usage Rate} = \frac{\text{FGA} + 0.44 \times \text{FTA} + \text{TOV}}{\text{MIN}} \times 100$$

  **Availability Threshold:** Filtering out players with $< 50$ games played ensures we only evaluate realistic, highly durable MVP candidates. 

  **🗂️ Project Structure**
  
  nba-mvp-predictor/
├── notebooks/
│   └── NBA_MVP_Prediction.ipynb
├── README.md
├── requirements.txt
└── .gitignore

**🛠️ How to Run**
1. Clone the Repository
   ```bash
   git clone https://github.com/adas1496/nba-mvp-predictor.git
   cd nba-mvp-predictor

2. Install Dependencies
pip install -r requirements.txt

3. Run the Notebook
Open notebooks/NBA_MVP_Prediction.ipynb in your environment and run all cells.
