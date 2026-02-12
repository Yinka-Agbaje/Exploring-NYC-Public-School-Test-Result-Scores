

# 🎓 NYC Academic Performance Audit: SAT Socio-Economic Trends
![Category: Exploratory Data Analysis](https://img.shields.io/badge/Category-Data_Integration_/_ETL-blue?style=for-the-badge)
![Tech: Variance Modeling](https://img.shields.io/badge/Tech-Multi--Format_Processing-orange?style=for-the-badge)

# Project overview
Analyzing academic performance is vital for educational stakeholders to allocate resources effectively. This project performs a **deep-dive audit** of SAT results across New York City’s five boroughs, identifying not only top-performing institutions but also the geographic variance that indicates educational inequality.

## 🎯 The Mission
The goal of this project was to identify systemic trends in underperformance across public schools by analyzing a dataset of over **50,000 student records**. Rather than just reporting numbers, I simulated an **audit workflow** to provide data-driven interventions for educational equity.

## 🛠️ Tech Stack & Methodology
Language: Python 3.10+
Libraries: Pandas (Vectorized operations), NumPy (Statistical computations), Matplotlib/Seaborn (Visualizing distribution)
Key Techniques: Data Aggregation, Lambda Functions for Feature Engineering, and Standard Deviation Analysis to measure performance volatility.

## 📊 Objectives & Findings
1. High-Performance Math BenchmarkingMetric: Filtered for schools achieving $\ge 80\%$ ($640+$ points) in Mathematics.Insight: Identified a elite cluster of schools, providing a benchmark for curriculum success that can be modeled in other districts.
2. Composite Score EngineeringAction: Engineered a new feature, total_SAT, by aggregating Math, Reading, and Writing scores to provide a holistic view of student success beyond specialized subjects.Top 10 Analysis: Ranked the city's highest-achieving schools to identify geographic "Education Hubs."
3. Borough-Level Variance Audit (The "Job-Ready" Insight)Method: Grouped data by borough to compute the Mean and Standard Deviation ($\sigma$).Critical Finding: Manhattan exhibited the highest variability in scores ($Std \ Dev \approx 230.29$).

**Business Impact** : High variance suggests a wide "achievement gap" within the same borough, highlighting where targeted government interventions are most needed compared to boroughs with more uniform performance.

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

## 👩‍💻 Author
Olayinka Agbaje| Data Scientist
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?style=flat&logo=linkedin)](www.linkedin.com/in/olayinka-agbaje-188102224) 
[![Email](https://img.shields.io/badge/Email-Contact-red?style=flat&logo=gmail)](mailto:olayinkaagbaje01@gmail.com)

---

### Run the notebook

```bash
jupyter notebook notebooks/analysis.ipynb

---

## ✅ Results


* **Top Math Schools:** e.g., `[School A, School B, …]`
* **Top 10 Total SAT Schools:** `[Manhattan]`
* **Borough with highest SAT variability:** `Manhattan (Avg SAT = 1340.13, Std Dev = 230.29)




