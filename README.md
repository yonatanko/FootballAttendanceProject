# ⚽ Football Attendance and Extreme Weather Analysis 🌧️

## 📌 Project Overview
This project investigates whether extreme weather conditions prior to a Premier League match impact stadium attendance. Using data from multiple seasons, we apply causal inference methods to estimate the Average Treatment Effect (ATE) of severe weather conditions on match attendance.

## 📂 Repository Structure
- 📜 `Data_prep.ipynb` - Preprocessing scripts for cleaning and structuring the dataset.
- 📊 `EDA.ipynb` - Exploratory Data Analysis (EDA) to understand key trends and distributions.
- 🤖 `models.ipynb` - Implementation of causal inference models for ATE estimation.

## 📊 Data
The dataset includes match attendance records, weather conditions, and various match-specific features from four English Premier League seasons: 2017/18, 2018/19, 2022/23, and 2023/24. Data sources include:
- ⚽ Football statistics websites
- 🌦️ Weather data via API
- 🏟️ Stadium metadata from Wikipedia

### 🔑 Key Features
- **📆 Match details**: Date, teams, stadium, league rankings
- **🌡️ Weather conditions**: Temperature, precipitation, wind speed, extreme weather indicator
- **👥 Attendance data**: Percentage of stadium capacity filled
- **🏆 Football context features**: Weekend match, holiday match, "Big 6" teams, close match indicators

## 🏗️ Methodology
We estimate ATE using various causal inference techniques:
- **Covariates-based methods**: S-Learner, T-Learner, Nearest Neighbor Matching
- **Propensity score-based methods**: Propensity Score Matching, Inverse Probability Weighting (IPW)
- **Evaluation techniques**: Propensity score overlap analysis, calibration curves

## 📈 Results
- All estimation methods suggest that extreme weather negatively impacts stadium attendance.
- The magnitude of the effect varies across methods but consistently shows a decline in attendance percentages.
- The study highlights the importance of considering weather conditions when analyzing match attendance trends.

## 🚀 Running the Code
1. Clone this repository:
   ```bash
   git clone https://github.com/yonatanko/FootballAttendanceProject.git
   ```
2. Navigate to the project folder:
   ```bash
   cd FootballAttendanceProject
   ```
3. Run Jupyter Notebook:
   ```bash
   jupyter notebook
   ```
4. Open and execute the notebooks in the following order:
   - 📜 `Data_prep.ipynb`
   - 📊 `EDA.ipynb`
   - 🤖 `models.ipynb`

## ✍️ Authors
- 🧑‍💻 Yonatan Koifman
- 👨‍💻 Daniel Mreeh
