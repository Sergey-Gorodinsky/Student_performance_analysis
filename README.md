

# Student Performance Analysis

Exploratory data analysis of 1_000 students
examining the relationship between study habits,
sleep patterns, online courses enrollment and
academic performance.


| | |
|---|---|
| Source | `https://www.kaggle.com/datasets/alhamdulliah123/student-learning-habits-and-exam-performance` |
| Size | 1,000 rows × 5 columns |
| Features | `daily_study_hours`, `online_courses_taken`, `avg_sleep_hours` |
| Target | `exam_score` range(40-100)|

---

<h1 align="center">Executive Summary</h1>

<img width="1389" height="1590" alt="histograms" src="https://github.com/user-attachments/assets/229e889e-5d61-413f-a424-777bfbf4ddf8" />


| Variable | Details |
|---|---|
| **daily_study_hours**| Uniform distribution - KDE is almost flat, no distinct peak. Skewness ≈ 0 - symmetrical. Range: 0.5 - 8 hours. No outliers |
| online_courses_taken | Uniform distribution - KDE is flat because data is discrete. Each value occurs ≈ 150 - 175 times. No outliers |
| **avg_sleep_hours** | Close to normal distribution - slightly bimodal (two small peaks near 5 and 7.5). Skewness: Weak left skew, slightly more students sleep less than average. Range: 4 - 9 hours. No outliers |
| **exam_score** | Bimodal distribution - two peaks: one around 50–55, the other around 80–85. Skewness ≈ 0. Range: 40 - 100. No outliers





<img width="1108" height="986" alt="pairplot" src="https://github.com/user-attachments/assets/db1fea43-2f0a-48d2-8dd3-11a62ff83147" />

**Observations:**
* All scatter plots show completely mixed color groups - no feature separates Low, Medium, and High performers.This confirms information from the correlation matrix: study hours, sleep, and online courses are equally distributed across all score groups.
* The KDE diagonal reveals that avg_sleep_hours is bimodal across all groups, suggesting sleep patterns are independent of performance.
* Conclusion: individual features alone cannot explain exam score.The dataset was generated independently of these features.


![alt text](images/correlations_heatmap.png)
Observations:
* No meaningful linear correlation was found between any feature indicating that study hours,
sleep, and online courses individually cannot predict exam performance through a linear relationship.



- **Bimodal score distribution** - two distinct peaks near 50 and 80; students cluster into weak and strong performers


- **Features are independent of performance** - Low, Medium, and High scorers have virtually identical study hours, sleep, and course enrollment
- **Equal segment distribution** - 33% of students in each score group, atypical for real academic data
- **Dataset is likely synthetic** - uniform feature distributions and near-zero correlations suggest scores were generated independently of the measured habits


## Examinations of perfomarnce factors

### Study time



### Does exam score increase with study time?
Answer: No

Mean exam scores across study groups range from 69.5 to 71.0 - 
a difference of only 1.5 points. Boxplots show near-identical 
distributions across all groups.

Study time has no meaningful effect on exam performance in this dataset.
This is consistent with datasat being synthetic




## Data Cleaning

---

1. Removed redundant colums
2. Checked column names for readability
3. Checked data types
4. Checked for duplicates
5. Checked for Nan values
6. Checked for outliers using IQR method
7. Checked for logical errors

---

## EDA Overview


| Section | Description |
|---|---|
| 1. General Data Information | Shape, dtypes, missing values, duplicates |
| 2. Univariate Analysis | Distributions, skewness, outliers |
| 3. Correlation Analysis | heatmap |
| 4. Pairplot | Multi-variable relationships by score group |
| 5. Performance Factors | Study time, sleep, courses vs exam score |
| 6. Student Segmentation | Low/Medium/High performer profiles |
| 7. Key Insights & Conclusion | Main findings and limitations |

---

