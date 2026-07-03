# Machine Learning Practices - 1

## Overview

This repository contains my hands-on Machine Learning practice focused on **Data Preprocessing**, **Exploratory Data Analysis (EDA)**, and **Feature Engineering**. The primary objective of this project is to understand how raw datasets are transformed into clean, structured, and machine-learning-ready data before training Machine Learning models.

Through this project, I practiced the essential preprocessing techniques used in real-world Data Science and Machine Learning workflows.

---

# Project Objectives

- Understand the Machine Learning preprocessing pipeline.
- Perform Exploratory Data Analysis (EDA).
- Clean and preprocess raw data.
- Handle missing values and duplicate records.
- Visualize important data insights.
- Apply encoding techniques.
- Perform Feature Engineering.
- Scale numerical features.
- Select the most relevant features.
- Prepare data for Machine Learning algorithms.

---

# Technologies Used

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

---

# Concepts Covered

## 1. Exploratory Data Analysis (EDA)

Exploratory Data Analysis is the process of understanding the dataset before building Machine Learning models.

### Performed:

- Understanding dataset structure
- Checking rows and columns
- Viewing dataset information
- Statistical summary
- Data distributions
- Correlation analysis
- Identifying patterns

### Purpose

EDA helps in understanding:

- Data quality
- Missing values
- Outliers
- Relationships between variables
- Feature distributions

---

## 2. Data Cleaning

Data cleaning improves the quality of data before model training.

### Tasks Performed

- Removed duplicate records
- Corrected inconsistent data
- Verified column data types
- Cleaned unnecessary information

### Why Data Cleaning?

Clean data improves model accuracy and reduces errors.

---

## 3. Handling Missing Values

Datasets often contain missing values that must be handled before training.

### Methods Used

- Checking null values
- Identifying incomplete records
- Preparing clean datasets

### Importance

Missing values may decrease model performance if ignored.

---

## 4. Data Visualization

Data visualization helps understand the dataset visually.

### Charts Used

- Histograms
- Box Plots
- Scatter Plots
- Correlation Heatmaps

### Benefits

- Detect trends
- Detect outliers
- Understand distributions
- Identify relationships

---

## 5. Label Encoding

Label Encoding converts categorical values into numerical values.

Example

Male → 0

Female → 1

Used for:

- Sex
- Smoker

---

## 6. One-Hot Encoding

One-Hot Encoding converts categorical columns into binary columns.

Example

Region

Northwest

Southeast

Southwest

becomes

Region_Northwest

Region_Southeast

Region_Southwest

This prevents Machine Learning models from assuming any order between categories.

---

## 7. Feature Engineering

Feature Engineering creates meaningful features from existing data.

### Implemented

BMI values were converted into BMI Categories using:

- Underweight
- Normal
- Overweight
- Obese

using

```python
pd.cut()
```

This improves data interpretability.

---

## 8. BMI Category Creation

BMI was categorized using the following ranges:

| BMI Range | Category |
|-----------|----------|
| Below 18.5 | Underweight |
| 18.5 – 24.9 | Normal |
| 25 – 29.9 | Overweight |
| Above 30 | Obese |

This is an example of Feature Engineering.

---

## 9. Feature Scaling

Machine Learning algorithms perform better when numerical features are on the same scale.

### Technique Used

StandardScaler

### Benefits

- Faster model convergence
- Better performance
- Removes scale differences

---

## 10. Feature Selection

Feature Selection identifies the most useful features for prediction.

### Techniques Practiced

- Correlation Analysis
- Chi-Square Test

### Benefits

- Reduces overfitting
- Improves accuracy
- Faster training
- Removes irrelevant features

---

## 11. Correlation Analysis

Correlation measures the relationship between numerical variables.

Correlation values range between

-1 → Negative Correlation

0 → No Correlation

+1 → Positive Correlation

Heatmaps were used to visualize correlations.

---

## 12. Chi-Square Test

Chi-Square Test measures the relationship between categorical variables.

Purpose

- Select important categorical features
- Remove less useful variables

---

# Machine Learning Workflow

Raw Dataset

↓

Exploratory Data Analysis

↓

Data Cleaning

↓

Handle Missing Values

↓

Data Visualization

↓

Encoding

↓

Feature Engineering

↓

Feature Scaling

↓

Feature Selection

↓

Machine Learning Ready Dataset

---

# Libraries Used

```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns

from sklearn.preprocessing import LabelEncoder
from sklearn.preprocessing import OneHotEncoder
from sklearn.preprocessing import StandardScaler
from sklearn.feature_selection import chi2
```

---

# Key Learnings

Through this project, I learned:

- Importance of clean data
- Data preprocessing pipeline
- Exploratory Data Analysis
- Feature Engineering
- Feature Selection
- Label Encoding
- One-Hot Encoding
- Standardization
- Correlation Analysis
- Chi-Square Feature Selection
- Preparing datasets for Machine Learning

---

# Future Work

Next, I will continue learning:

- Supervised Learning
- Regression Algorithms
- Classification Algorithms
- Model Evaluation
- Model Training
- Hyperparameter Tuning
- Machine Learning Projects
- Deep Learning

---

# Repository Structure

```
Machine-Learning-Practices-1/
│
├── Dataset/
├── Images/
├── ML_Tasks.ipynb
├── README.md
└── requirements.txt
```

---

# Author

**Vikrant Vinayak Sutar**

Passionate about **Data Analytics, Machine Learning, Artificial Intelligence, and Python Development**.

Currently building real-world Machine Learning projects while continuously improving my skills in Data Science and AI.

---

## If you found this repository helpful, consider giving it a ⭐.
