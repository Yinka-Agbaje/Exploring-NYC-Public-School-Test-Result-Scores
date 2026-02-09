

# 🎓 NYC Academic Performance Audit: SAT Socio-Economic Trends
      Exploratory Data Analysis (EDA) & Variance Modeling

# Project overview
Analyzing academic performance is vital for educational stakeholders to allocate resources effectively. This project performs a **deep-dive audit** of SAT results across New York City’s five boroughs, identifying not only top-performing institutions but also the geographic variance that indicates educational inequality.

## 🎯 The Mission
The goal of this project was to identify systemic trends in underperformance across public schools by analyzing a dataset of over **50,000 student records**. Rather than just reporting numbers, I simulated an **audit workflow** to provide data-driven interventions for educational equity.


## 🧭 Project Objectives
1. **Load the dataset** (`schools.csv`).
2. Identify **high-performing math schools** (≥ 80% of max score).
3. Compute a new **total SAT score** (Math + Reading + Writing).
4. Get the **Top 10 schools by total SAT**.
5. Group schools by **borough**, compute average SAT & standard deviation.
6. Identify the **borough with the highest variation** in SAT scores.

## 📂 Dataset

* **File:** `schools.csv`
* **Columns used:**

  * `school_name`
  * `borough`
  * `average_math`
  * `average_reading`
  * `average_writing`

https://data.cityofnewyork.us/Education/2012-SAT-Results/f9bf-2cp4/about_data


## 🗂️ Repository Structure
nyc-sat-analysis/
├── data/
│   └── schools.csv
├── notebooks/
│   └── analysis.ipynb
├── reports/
│   └── figures/   
├── src/
│   └── analysis.py
├── README.md
├── requirements.txt
└── .gitignore


**requirements.txt**
pandas>=2.0
numpy
jupyter

### Run the notebook

```bash
jupyter notebook notebooks/analysis.ipynb
```

---

## 📊 Analysis Overview

### 1. High-Performing Math Schools

* Selected schools with **average\_math ≥ 640 (80% of 800 max)**.
* Sorted results to rank schools by math performance.

### 2. Top 10 Schools by Total SAT

* Computed:

  total_SAT = average_math + average_reading + average_writing
  ```
* Ranked all schools by total SAT and extracted the **top 10 performers**.

### 3. Borough Statistics

* Aggregated by borough:

  * Number of schools
  * Mean total SAT
  * Standard deviation of SAT scores
* Identified borough with **highest variability** in scores.

---

## ✅ Results


* **Top Math Schools:** e.g., `[School A, School B, …]`
* **Top 10 Total SAT Schools:** `[Manhattan]`
* **Borough with highest SAT variability:** `Manhattan (Avg SAT = 1340.13, Std Dev = 230.29)

---

## 👩‍💻 Author

Yinka Agbaje
* [LinkedIn]([https://www.linkedin.com/in/olayinka-agbaje-188102224/]) | [Email](olayinkaagbaje01@gmail.com)



