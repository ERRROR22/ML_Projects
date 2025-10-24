# 🏏 IPL Score Predictor

## 🚀 Project Overview
The **IPL Score Predictor** is a machine learning project that predicts the final innings score in an IPL match based on gameplay data from early overs. It uses historical IPL match data to train regression models that forecast the total runs scored.

## 📊 Dataset Description
The dataset contains ball-by-ball IPL match details including teams, runs, wickets, overs, and performance in the last 5 overs. Only consistent IPL teams over seasons are used after filtering irrelevant columns.

## 🔧 Data Preprocessing
- Removed irrelevant columns like venue, date, batsman, and bowler.
- Filtered data to include matches between 8 consistent teams.
- Dropped initial overs to focus on more predictive overs.
- Used label encoding and one-hot encoding on categorical features.

## 🧠 Model Training
Trained multiple regression models:
- Decision Tree Regressor
- Linear Regression
- Random Forest Regressor
- Support Vector Regressor
- KNN Regressor

Split dataset into 80% training and 20% testing.

## 📈 Evaluation Metrics
Evaluated models using:
- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- R² Score for training and testing

## 🏆 Best Model
**Random Forest Regressor** showed the highest accuracy and lowest error and is saved as `mlmodel.pkl` for future prediction use.

## 💻 Usage
Use the `scorepredict()` function with inputs:
to predict the final innings score.

## 🔍 Example Predictions
| Batting Team | Bowling Team | Overs | Current Score | Predicted Final | Actual Final |
|--------------|--------------|-------|---------------|-----------------|--------------|
| Delhi Daredevils | CSK | 10.2 | 68/3 | 148 | 147 |
| Mumbai Indians | Kings XI Punjab | 12.3 | 113/2 | 186 | 176 |

## 📚 Libraries Used
- Python 3.x
- NumPy, Pandas
- Scikit-learn
- Matplotlib
- Pickle

## 🎯 Future Work
- Deploy as a real-time web app or dashboard.
- Add more features such as player stats and weather.
- Experiment with deep learning models for better accuracy.

## ✍️ Author
Developed by a Computer Science Engineering student focusing on practical ML applications in sports analytics.
[Ritik Sharma]
---

Feel free to ask if you want me to generate a detailed academic report version too!
