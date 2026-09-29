# 🧠 Stress Level Analysis

## 📌 Project Overview

This project analyzes employee wellness survey and activity data to understand **employee stress levels** and identify patterns related to work hours, sleep, exercise, caffeine intake, department, age, and gender.

The analysis uses **Power BI** to create an interactive dashboard that helps identify stress patterns and high-stress employee groups.

---

## 🎯 Objectives

* Analyze employee stress levels.
* Identify factors associated with higher stress.
* Compare stress levels across departments.
* Analyze stress trends over time.
* Examine the relationship between work hours and stress.
* Analyze the relationship between sleep hours and stress.
* Identify employees with very high stress levels.

---

## 📊 Dataset

The dataset contains the following fields:

* EmployeeID
* Department
* Age
* Gender
* WorkHours
* SleepHours
* ExerciseHours
* CaffeineIntake
* StressLevel
* DateRecorded

**StressLevel:**
1 = Low
2 = Low
3 = Medium
4 = High
5 = Very High

---

## 🛠️ Tools & Technologies

* **Power BI**
* **DAX**
* **Microsoft Excel**
* **Data Visualization**
* **Data Analysis**

---

## 📈 Key KPIs

The dashboard includes:

* **Average Stress Level**
* **High Stress %**
* **Average Sleep Hours**
* **Average Work Hours**
* **Average Sleep vs Work Ratio**

---

## 📊 Dashboard Visualizations

The Power BI dashboard includes:

### 1. Average Stress by Department

A column chart comparing average stress levels across departments.

### 2. Stress Level Trend

A line chart showing changes in average stress levels over time.

### 3. Work Hours vs Stress Level

A scatter plot analyzing the relationship between working hours and stress levels.

### 4. Stress Level Distribution

A donut chart showing the distribution of Low, Medium, and High stress levels.

### 5. High-Stress Employees

A table highlighting employees with:

* StressLevel = 5
* SleepHours < 5

---

## 🎛️ Dashboard Filters

Interactive slicers are provided for:

* Department
* Gender
* Age Group

---

## 🧮 DAX Measures

Important measures used in the analysis include:

```DAX
Avg Stress Level =
AVERAGE(Stress analysis Data[StressLevel])
```

```DAX
High Stress % =
DIVIDE(
    CALCULATE(
        COUNTROWS(StressData),
        Stress analysis Data[StressLevel] >= 4
    ),
    COUNTROWS(StressData),
    0
)
```

```DAX
Avg Sleep Hours =
AVERAGE(Stress analysis Data[SleepHours])
```

```DAX
Avg Work Hours =
AVERAGE(Stress analysis Data[WorkHours])
```

```DAX
Avg Sleep vs Work Ratio =
DIVIDE(
    [Avg Sleep Hours],
    [Avg Work Hours],
    0
)
```

---

## 💡 Key Insights

* Employees working longer hours tend to show higher stress levels.
* Employees with fewer sleep hours are more likely to have higher stress levels.
* Stress levels vary across departments.
* Higher stress levels are observed among employees with lower sleep duration.
* Employees with StressLevel = 5 and SleepHours < 5 represent a high-stress group requiring attention.

---

## 📁 Project Structure

```text
Stress-Level-Analysis/
│
├── Dataset/
│   └── Stress_Level_Data.xlsx
│
├── PowerBI/
│   └── Stress_Level_Analysis.pbix
│
├── Images/
│   └── Dashboard_Screenshot.png
│
└── README.md
```

---

## 📌 Conclusion

The Stress Level Analysis dashboard provides an interactive view of employee stress patterns and their relationship with work and sleep factors. The analysis can help organizations identify patterns that may require further attention and support employee well-being.

---

## 👩‍💻 Author

**Y. Ramyakrishna**

Aspiring Data Analyst | Power BI | SQL | Excel | Python
