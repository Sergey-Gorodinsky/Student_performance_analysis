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

## Key Insights

- **No linear correlations found** - No
meaningfull correlation between features
- **Bimodal score distribution** - two distinct peaks near 50 and 80; students cluster into weak and strong performers
- **Features are independent of performance** - Low, Medium, and High scorers have virtually identical study hours, sleep, and course enrollment
- **Equal segment distribution** - 33% of students in each score group, atypical for real academic data
- **Dataset is likely synthetic** - uniform feature distributions and near-zero correlations suggest scores were generated independently of the measured habits


## Limitations

- Dataset appears synthetically generated - findings may not reflect real student behavior
- Key predictors likely missing: attendance, prior GPA, motivation, background ...
- No causal inference possible from correlation analysis alone




---

## Requirements

```
jupyter
pandas
numpy
matplotlib
seaborn
```

---


## Project Structure

```
Student_Perfomance_Analysis/
│
├── data/
│   ├── raw/
│   │   └── student_learning_habits_dataset.csv   # Original dataset
│   └── processed/
│       └── students_data.csv                     # Cleaned dataset
│
├── images/                                        # All visualizations
│   ├── histograms.png
│   ├── correlations_heatmap.png
│   ├── pairplot.png
│   ├── exam_score_and_study_hours.png
│   ├── exam_score_and_courses.png
│   ├── exam_score_and_sleep.png
│   ├── segments_distribution.png
│   └── segments.png
│
├── notebooks/
│   ├── data_cleaning.ipynb                       # Data preprocessing
│   └── eda.ipynb                                 # Full EDA
│
├── .gitignore
├── requirements.txt
└── README.md
```

---

