# UBER_DATA_ANALYSIS
# 🚗 Uber Rides: Exploratory Data Analysis (EDA)
![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Pandas](https://img.shields.io/badge/Library-Pandas-orange)
![Matplotlib](https://img.shields.io/badge/Library-Matplotlib-green)

## 📌 Project Overview
This project involves a deep-dive analysis of Uber ride data to uncover patterns in travel behavior, trip purposes, and peak usage times. By transforming raw trip logs into visual insights, this analysis helps understand how users utilize ride-sharing services for business vs. personal needs.

## 🛠️ Tech Stack
* **Language:** Python
* **Libraries:** Pandas, NumPy (Data Manipulation), Matplotlib, Seaborn (Visualization)
* **Tools:** Jupyter Notebook, Git/GitHub

## 🧹 Data Cleaning & Preprocessing
To ensure high-quality insights, the raw data underwent several transformation steps:
* **Handling Missing Values:** Imputed missing values in the `PURPOSE` column with "NOT" to maintain dataset integrity.
* **DateTime Transformation:** Converted `START_DATE` and `END_DATE` into Python DateTime objects for temporal analysis.
* **Feature Engineering:** * Extracted `date` and `hour` from timestamps.
    * Categorized trips into **Morning, Afternoon, Evening, and Night** segments using binning.
* **Deduplication:** Identified and removed duplicate records to prevent skewed results.

## 📊 Key Insights & Observations
* **Trip Categorization:** The vast majority of trips are categorized as **Business**, with specific high-frequency purposes like "Meetings" and "Meal/Entertain."
* **Peak Usage:** Analysis of the `day-night` feature reveals peak demand periods, showing when users are most active.
* **Distance Metrics:** Explored the distribution of `MILES` to distinguish between short city hops and long-distance travel.
* **Location Hotspots:** Identified the top 10 most frequent starting and stopping points.

## 📈 Visualizations
The notebook includes high-quality plots such as:
* **Count Plots:** Distribution of trips by category (Business vs. Personal).
* **Time-Series Analysis:** Hourly trends showing the busiest times of the day.
* **Purpose Distribution:** A breakdown of why users are booking rides.

## 🚀 How to Run
1. Clone this repository:
   ```bash
   git clone [https://github.com/your-username/uber-rides-analysis.git](https://github.com/your-username/uber-rides-analysis.git)
   pip install pandas numpy matplotlib seaborn
   jupyter notebook "uber rides data analysis.ipynb"
