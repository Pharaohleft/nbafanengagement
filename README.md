# NBA Team Performance & Fan Engagement Analysis


✅ Project 3 Recap: Role/Archetype Comparison & Career Alignment
Objective: Compare young stars (Tatum, Edwards) to NBA legends based on stats and career trajectory up to current season number.

🔹 Player-to-GOAT Alignment (Season-by-Season)
Compared Tatum's stats season-by-season with:

Michael Jordan

Kobe Bryant

Other GOATs (planned)

✅ Matched based on career season number (not age or peak years)
✅ Ensured fair comparison: Tatum’s first 6 seasons vs first 6 seasons of each GOAT

🔹 Radar Charts: Stat Comparison
Compared key per-game stats using radar charts:

PPG, APG, RPG, FG%, 3P%, MIN

Fixed multiple errors:

Different feature counts across players

Index mismatch issues

Invalid FG%/3P% (missing or zero-filled → corrected)

🛠️ Radar charts were eventually scrapped due to interpretability issues. You decided to focus on plain numeric comparison.

✅ Project 4 Recap: Multi-Season Time-Series Forecasting
🔹 Forecasting with Prophet
Forecasted PPG growth for Anthony Edwards using Prophet

Then tested Prophet’s accuracy by training on MJ’s first 5 seasons → compared prediction with actual values

Result:

Prophet overestimated MJ’s peak

RMSE ≈ 4.81

🔹 Prophet vs ARIMA for Edwards
Prophet forecasted next 2 seasons of Edwards → RMSE = 0.94

ARIMA forecasted same → RMSE = 2.43
✅ Prophet outperformed ARIMA for Edwards

✅ Visualization Work
🔹 Clean Line Charts for Per-Game Stats
Created clean charts for:

Michael Jordan's first 6 seasons (PPG, APG, RPG)

Anthony Edwards’ NBA seasons (PPG, APG, RPG)

🔄 These can be reused for any player or combined plots

✅ Key Errors We Overcame
❌ KeyError: 'AGE' → fixed by using actual column name

❌ Radar chart dimension mismatches → fixed by aligning features manually

❌ Prophet overfitting small sample → tuned seasonality & changepoint

❌ Misleading visualizations → switched to clearer line plots

❌ Prophet vs ARIMA testing → evaluated with RMSE comparison



This project analyzes NBA teams using data-driven insights across:

- Game performance
- Fan engagement metrics
- Financial indicators

It includes:

✅ **Classification Model**: Predicts if a team has a winning record based on engagement and performance metrics.  
✅ **Regression Model**: Predicts the number of wins for each team.  
✅ **KMeans Clustering**: Groups teams by similar characteristics (performance & fanbase).  
✅ **PCA Visualization**: See how teams cluster in 2D!

---

## Technologies Used

- **Python** (pandas, sklearn, seaborn, matplotlib)
- **Jupyter Notebook / Colab** for interactive analysis
- **PCA** for dimensionality reduction
- **KMeans** for clustering analysis

---

## Data

- 📁 Dataset: `nba.xlsx` (custom dataset with performance, financial, and fan data).

---

## Key Insights

- Teams cluster into 3 distinct groups by performance and engagement.
- High fan engagement metrics (social media, attendance) correlate with strong performance.
- Regression and classification models achieved excellent accuracy (see notebook).

---

## To Run

1️⃣ Clone the repo:  
```bash
git clone https://github.com/yourusername/nba-team-analytics.git
# nbafanengagement
Tableau dashboard analyzing NBA team fan engagement via attendance, wins, and social media
