

# 📊 Academic Pressure Analysis Project

## 📝 Project Overview

This project focuses on analyzing the factors contributing to academic stress among students. By exploring a dataset of student responses, this analysis investigates correlations between study environments, peer pressure, lifestyle habits, and overall stress levels to identify behavioral patterns and common coping mechanisms.

## 🎯 Objectives

The primary goals of this analysis were to:

1. 
**Demographic Analysis:** Understand the distribution of students across different academic stages (High School, Undergraduate, Post-graduate).


2. 
**Behavioral Insights:** Identify the most prevalent **Coping Mechanisms** used by students.


3. **Correlation Study:** Determine if there are statistically significant relationships between:
* Study Environment and Academic Pressure at home.


* Peer Pressure and Stress Levels.


* Academic Stage and Coping Mechanisms.




4. 
**Temporal Analysis:** Analyze if stress levels fluctuate based on the day of the week or specific months (July vs. August).



## 🛠️ Methodology & Workflow

### 1. Data Cleaning & Preprocessing

* 
**Handling Missing Data:** Identified and removed rows containing null values to ensure analysis accuracy (`dropna`).


* 
**Renaming Features:** Renamed verbose column names for better readability (e.g., changed *"What coping strategy..."* to `Coping_Mechanism`).


* **Data Transformation (Mapping):** Converted numerical scales (1-5) into categorical labels for better interpretation:
* 
*Peer Pressure:* 1 → 'Very Low' ... 5 → 'Very High' .


* 
*Academic Pressure:* 1 → 'No Pressure' ... 5 → 'Extreme Pressure' .




* 
**Feature Engineering:** Extracted `Month`, `Year`, and `Day_Name` from the `Timestamp` column to facilitate time-series analysis .



### 2. Exploratory Data Analysis (EDA)

* Visualized the distribution of academic stages using Bar Charts.


* Analyzed the composition of stress levels using Pie Charts.


* Identified the most common coping mechanisms via frequency analysis.



### 3. Statistical Analysis

Advanced statistical tests were performed using `scipy.stats` to validate hypotheses:

* **Chi-Square Test of Independence:** Used to examine relationships between categorical variables.
* 
*Result:* Found a significant relationship between **Peer Pressure** and **Stress Levels** (P-value  0).


* 
*Result:* Confirmed a relationship between **Academic Stage** and **Coping Mechanisms**.




* **T-Test:** Used to compare the means of stress scores between July and August.
* 
*Result:* P-value > 0.05, indicating no statistically significant difference in average stress between these two months.





## 📊 Key Findings

* 
**Demographics:** The majority of the dataset consists of **Undergraduate** students.


* 
**Coping Strategies:** **"Problem Solving"** is the most widely adopted mechanism, followed by "Emotional Release".


* 
**Peer Pressure Impact:** There is a direct and significant correlation where students facing "Very High" peer pressure report "Overwhelming" stress levels.


* 
**Environmental Factors:** A "Disrupted" study environment is statistically linked to higher academic pressure from home.



## 🧰 Tools & Technologies

* **Language:** Python
* **Libraries:**
* 
**Pandas & NumPy:** Data manipulation and cleaning.


* 
**Matplotlib & Seaborn:** Data visualization (Heatmaps, Count plots, Box plots).


* 
**SciPy:** Statistical testing (Chi-Square, T-test).





---
