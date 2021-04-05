# Project 5: Absenteeism-at-Work

---

## Project Overview

- Objective : 
  - **To Predict Absenteeism at Company during Worktime**
  - to integrate **Python, SQL, and Tableau**
- Classification Problem
- Data cleaning and Data preprocessing
- Exploratory Data Analysis
- **Logistic Regression Model** Training and Prediction
- Inteprating its Odd Ratios and Coefficients
- Integrating Model with SQL and Tableau


![](https://github.com/SidSolanki28/Absenteeism-at-Workplace/blob/master/images/images.jpeg)


---
## Go Through Links

[Github Link](https://github.com/SidSolanki28/Absenteeism-at-Work)

---
## About Project

Machine Learning Classification model is developed to predict absenteeism at company during work time. This helps in improving decision making by reorganising work process to avoid lack of productivity and increase quality of work.

Integrated Python, SQL, and Tableau which are three of the most widely used tools in the world of data science. Python is the leading programming language; SQL is the most widely used means for communication with database systems; Tableau is the preferred solution for data visualization;

To put it simply – SQL helps us store and manipulate the data we are working with, Python allows us to write code and perform calculations, and then Tableau enables beautiful data visualization. A well-thought-out integration stepping on these three pillars could save a business millions of dollars annually in terms of reporting personnel.

---
## Code and Resources used

- Python version: 3.7.6
- Packages: Pandas, Numpy, Seaborn, Matplotlib, Scikit, Pymysql
- Resources used:

* Udemy : https://udemy.com/course/python-sql-tableau-integrating-python-sql-and-tableau
* Machine Learning Mastery : https://machinelearningmastery.com/logistic-regression-for-machine-learning/

---
## Web Scraping

Dataset URL: https://archive.ics.uci.edu/ml/datasets/Absenteeism+at+work

Attribute Information:

1. Individual identification (ID)
2. Reason for absence (ICD).
3. Month of absence
4. Day of the week (Monday (2), Tuesday (3), Wednesday (4), Thursday (5), Friday (6))
5. Seasons
6. Transportation expense
7. Distance from Residence to Work (kilometers)
8. Service time
9. Age
10. Work load Average/day 
11. Hit target
12. Disciplinary failure (yes=1; no=0)
13. Education (high school (1), graduate (2), postgraduate (3), master and doctor (4))
14. Son (number of children)
15. Social drinker (yes=1; no=0)
16. Social smoker (yes=1; no=0)
17. Pet (number of pet)
18. Weight
19. Height
20. Body mass index
21. Absenteeism time in hours (target)

---
## Data Cleaning

There is no missing values in data.

---
## EDA

I looked at the distributions of the data and the value counts for the various categorical variables. Below are a few highlights :


![](https://github.com/SidSolanki28/Absenteeism-at-Workplace/blob/master/images/download%20(1).png)

![](https://github.com/SidSolanki28/Absenteeism-at-Workplace/blob/master/images/download%20(2).png)


---
## Model Building

### Logistic Linear Regression

Logistic regression is named for the function used at the core of the method, the logistic function.
Below is an example logistic regression equation:

y = e^(b0 + b1*x) / (1 + e^(b0 + b1*x))

Where y is the predicted output, b0 is the bias or intercept term and b1 is the coefficient for the single input value (x). Each column in your input data has an associated b coefficient (a constant real value) that must be learned from your training data.

The logistic function, also called the sigmoid function

---
## Model Prediction

| Features| Coefficients | Odds Ratio 
| ----------- | ----------- | --------- |
| Reason C | 1.716629 | 5.565735 |
| Reason A | 1.559403 | 4.755983 |
| Transportation expense	| 0.701718	| 2.017215 |
|	Social drinker | 0.588378	| 1.801065 |
|	Weight	| 0.586728 | 1.798096 | 

---
## Model Performance

| Label | precision | recall |  f1-score 
| ----------- | ----------- | --------- | ------- |
| 0 | 0.81 | 0.77 | 0.79 |
| 1 | 0.69 | 0.74 | 0.72 |
| accuracy |  |   | 0.76 |    

## Conclusion

After analyzing its Odd Ratios and Coefficients, we predict

- Reason A and C has most weightage

Therefore, reasons like poisoning, injuries and various diseases are most common reasons for absenteeism.

- Also, Transport is also an issue for an employee to get absent for hours.

- Also, Disciplinary failure has highly negative coefficient means if there is no discipine penalty, there is more chance that employee become present in working hours.

---

## Further Improvements

Working on SQL and Tableau Integration
