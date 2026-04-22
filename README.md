# 🏋️ Strength Training Progress Analysis
### Analysis of strength training data featuring 1RM tracking and equipment-normalized volume metrics.

## Overview
This project involves a comprehensive analysis of strength training data. The primary objective was to move beyond raw "plate weight" tracking to understand true mechanical workload, training distribution, and progree. By implementing custom feature engineering to account for equipment base weights (Barbells, EZ-bars) and body weight, I normalized the data to track **Total Training Volume** and **Estimated 1-Rep Max (1RM)** trends over time.

## 📊 Visual Analysis & Observations

### 1. Training Volume: Total vs. Added Volume
This visualization highlights the gap between the Added Volume (including bar weight) against Total Volume (including bar and body weight). It demonstrates the importance of data normalization in fitness tracking.
<img width="839" height="351" alt="Screenshot 2026-04-22 at 15 16 04" src="https://github.com/user-attachments/assets/fb7ac1b1-83ef-41ca-af10-f5ad232f032c" />

### 2. Exercise Intensity Heatmap
This heatmap identifies the "Intensity Zones" of the program, showing where the most volume is being accumulated .
<img width="840" height="586" alt="Screenshot 2026-04-22 at 15 17 04" src="https://github.com/user-attachments/assets/e1c4a952-4be5-4c5e-a3b9-85ad7c60cdd9" />


## Key Insights
* **Data Normalization:** Raw workout logs often ignore the 20kg barbell or 80kg body weight base. I created a mapping system to "correct" these values, providing a high-fidelity view of the true physical stimulus.
* **Strength Progression (1RM):** Applied the **Brzycki Formula** ($Weight \times (36 / (37 - Reps))$ ) to normalize sets of varying rep ranges, allowing for a standardized tracking of absolute strength gains.
* **Visual Dejunking:** Following data visualization best practices, I removed unnecessary chart spines and used a distinct color palette (Teal vs. Coral) to maximize the "Data-to-Ink" ratio and improve readability.

## Technical Skills Demonstrated
* **Advanced Feature Engineering:** Creating logic-based columns for weight offsets based on exercise equipment categories.
* **Data Hygiene & Wrangling:** Standardizing categorical mislabeling and handling temporal data types using **Pandas**.
* **Exploratory Data Analysis (EDA):** Aggregating daily and weekly metrics to identify performance plateaus and progressive overload.
* **Professional Visualization:** Utilizing **Matplotlib** and **Seaborn** to create complex time-series subplots and intensity heatmaps.

## Data Source
The dataset consists of personal training logs captured over a longitudinal period, exported from a tracking application and cleaned for analysis.
