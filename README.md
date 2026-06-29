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

## Executive Summary

- **No linear correlations found** - No
meaningfull correlation between features. The dataset
was synthetically generated. Dataset lacks correlations and
connection between different features.
<img width="1554" height="605" alt="correlations_heatmap" src="https://github.com/user-attachments/assets/186789e9-63c3-4f88-82ef-f193a4bc7d03" />
No meaningful linear correlation exists between any feature and exam_score.
- All Pearson values are close to 0, indicating that study_hours,
  sleep, and online courses individually cannot predict exam performance through a linear relationship.


  // TODO rest
