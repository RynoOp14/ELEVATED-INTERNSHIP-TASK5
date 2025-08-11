Titanic - Exploratory Data Analysis (EDA)
📌 Project Overview
This project is part of Task 5 in my Data Analyst Internship. The objective was to perform Exploratory Data Analysis (EDA) on the Titanic dataset to discover patterns, relationships, and trends related to passengers’ survival chances.

The Titanic dataset is a classic beginner-friendly dataset from Kaggle, containing details of passengers aboard the RMS Titanic, such as age, gender, class, ticket fare, and survival status.

📂 Dataset Files
This repository contains the following files:

train.csv → Main dataset with survival labels (used for EDA)

test.csv → Passenger data without survival labels (used for prediction in ML tasks)

gender_submission.csv → Example submission file from Kaggle

task5.ipynb → Jupyter Notebook containing the entire EDA process

📊 EDA Process

1. Importing Libraries & Loading Data
Loaded the dataset using Pandas

Displayed first few rows with .head() for initial understanding

2. Data Inspection
.info() to view data types and non-null counts

.describe() for statistical summary

.isnull().sum() to check missing values

3. Handling Missing Values
Filled missing Age values with the median

Filled missing Embarked values with the mode

Created new column HasCabin (1 if cabin info exists, else 0) to use instead of the mostly empty Cabin column

4. Univariate Analysis
Count plots for Survived and Pclass

Histograms for Age and Fare distributions

5. Bivariate Analysis
Survival rate by Gender, Passenger Class, Embarked Port, and Cabin availability

Bar plots to visualize differences

6. Multivariate Analysis
Count plot showing combined effect of Pclass and Sex on survival

7. Correlation Analysis
Converted categorical columns (Sex, Embarked) to numeric

Created correlation matrix and plotted with a heatmap

8. Outlier Detection
Boxplots for Age and Fare to identify extreme values

🔍 Key Insights
Gender: Women had a much higher survival rate (~74%) compared to men (~19%).

Class: Higher-class passengers (1st class) survived more often than lower-class passengers.

Fare: Higher ticket fare correlated positively with survival chances.

Cabin: Passengers with recorded cabin numbers had better survival rates.

Age: Children had a slightly better chance of survival compared to adults.

🛠 Tools & Libraries Used
Python

Pandas → Data manipulation

NumPy → Numerical operations

Matplotlib & Seaborn → Data visualization

Jupyter Notebook
