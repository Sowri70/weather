# 🌤️ Weather Data Analysis

## 📘 Project Overview
This project explores and analyzes a weather dataset using **Python (Jupyter Notebook)** and **MySQL**.  
The main goal is to understand data patterns, clean the dataset, and visualize relationships between weather variables such as temperature, ozone levels, solar radiation, and wind speed.

---

## 🧩 Steps Involved

### 1. Data Loading
- Loaded **`weather_data.csv`** into **Jupyter Notebook** using `pandas`.
- Connected to **MySQL** for data storage and retrieval.
- Verified successful data import using `df.head()` and database queries.

---

### 2. Exploratory Data Analysis (EDA)

#### 🔹 Data Cleaning
- **Removed duplicates** to ensure data integrity.  
- **Dropped two unnecessary columns** that didn’t add analytical value.  
- **Renamed column:** `Solar.R` → `Solar`.  
- **Standardized column names** to lowercase for consistency.  
- **Corrected date format** to `YYYY-MM-DD` using `pd.to_datetime()`.

#### 🔹 Data Summary
- Used `df.info()`, `df.describe()`, and `df.isnull().sum()` to understand data types and check for missing values.

---

### 3. Data Visualization

#### 📊 Univariate Analysis
- **Box Plot (Ozone):** Identified outliers and visualized ozone distribution.  
- **Histogram (Wind):** Examined the frequency distribution of wind speeds.  
- **Distribution & Violin Plots (Solar):** Compared solar radiation spread and symmetry.

#### 📈 Bivariate Analysis
- **Scatter Plot (Ozone vs Temperature):** Observed positive correlation — higher temperatures often align with higher ozone levels.  
- **Pairplot (Weather Variables):** Explored interrelationships between all numeric variables.

#### 🌡️ Heat Map
- Created a **correlation heatmap** for `temp`, `day`, `wind`, `solar`, and `ozone` using `seaborn.heatmap()`.  
- Provided insights into which variables are most closely related.

---

## 🛠️ Tools & Libraries
- **Python:** pandas, matplotlib, seaborn, numpy  
- **Database:** MySQL  
- **Environment:** Jupyter Notebook  

---

## 🧠 Key Insights
- Data cleaning improved the dataset’s reliability.  
- Ozone values showed notable outliers requiring further analysis.  
- Solar radiation and temperature displayed moderate correlation with ozone.  
- The heatmap and pairplot revealed consistent patterns in seasonal variations.

---

## 📎 Conclusion
This project demonstrates a complete data analysis workflow — from importing raw data to cleaning, visualization, and deriving insights.  
It serves as a foundation for **predictive modeling**, **climate trend analysis**, or **environmental research**.

---

**Author:** Rajan Sowri  
**Environment:** Python 3.11 | Jupyter Notebook | MySQL  
**Date:** October 2025
