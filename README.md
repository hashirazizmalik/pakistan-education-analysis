# 📊 Pakistan Education Crisis: Data Analysis & Insights

## 📝 Project Overview
Despite decades of government programs and international aid, Pakistan faces a severe education crisis characterized by high dropout rates and significant gender disparities. 

This project explores historical World Bank education data (1970–2018) to move beyond simply observing dropout rates and instead identify **root causes** and **predictive trends**. Using Python, the analysis investigates the teacher-student pipeline, the systemic "brain drain" to higher education, and the true timeline of economic investments in literacy.

## 🛠️ Tools & Technologies
* **Language:** Python
* **Data Cleaning & Wrangling:** Pandas, NumPy (Handling missing data via linear interpolation and forward/backward filling)
* **Visualization:** Matplotlib, Seaborn (Dual-axis charts, custom funnel visualizations)
* **Machine Learning & Stats:** Scikit-Learn (Simple Linear Regression), Pearson Cross-Correlation
* **Dataset:** World Bank Education Indicators (Pakistan)

---

## 🔍 Key Findings & Executive Summary

### 1. The "Teacher-Student" Pipeline
**Question:** *Does a lack of female teachers correlate with the high dropout rate of female secondary students?*
* **Insight:** Yes. By plotting the percentage of female secondary teachers against the Gender Parity Index (GPI) of female students, the data reveals a near-perfect **Pearson correlation of 0.965**. 
* **Conclusion:** Families are significantly more likely to keep adolescent daughters in secondary school if the institution has adequate female representation on the teaching staff.

*(Insert your dual-axis teacher/student chart here by uploading the image to GitHub and using this syntax: `![Teacher Correlation](teacher_student_correlation.png)` )*

### 2. The Higher Education "Brain Drain" Funnel
**Question:** *How much of the population actually makes it to university?*
* **Insight:** Normalizing the gross enrollment ratios to a base cohort of 100 students reveals a massive leak in the education pipeline. For every **100 students** that enter primary school, only **47** transition to secondary school, and a mere **12** make it to tertiary (university) education.
* **Conclusion:** Government focus on building universities will be ineffective without first addressing the massive 53% attrition rate occurring at the secondary school level.

*(Insert your funnel chart here: `![Brain Drain Funnel](brain_drain_funnel.png)` )*

### 3. The Economic Impact Analysis (Money vs. Literacy)
**Question:** *Does government funding directly improve youth literacy, and how long does it take?*
* **Insight:** Education funding is highly volatile. More importantly, cross-correlation analysis proves that government expenditure does *not* yield immediate results. Testing time lags from 0 to 10 years showed that the impact of education spending on youth literacy peaks at exactly a **10-year lag**.
* **Conclusion:** Education investment is a long-term economic engine. Funding allocated today takes approximately an entire decade to manifest as measurable youth literacy improvements.

*(Insert your lag correlation chart here: `![Lag Correlation](lag_correlation.png)` )*

---

## 📂 Repository Structure
* `1.ipynb` - Initial data exploration, cleaning (imputation), and predictive baseline modeling.
* `2.ipynb` - The Teacher-Student Pipeline Analysis (Correlation & Dual-Axis visualization).
* `3.ipynb` - The Brain Drain Forecast (Custom Funnel Chart engineering).
* `4.ipynb` - The Economic Impact Analysis (Time-Series Cross-Correlation and Lag mapping).
* `education_pak.csv` - The raw World Bank dataset.

## 🚀 How to Run the Code
1. Clone this repository: `git clone https://github.com/hashirazizmalik/pakistan-education-analysis.git`
2. Ensure you have the required libraries installed: `pip install pandas numpy matplotlib seaborn scikit-learn`
3. Open the `.ipynb` notebooks in Jupyter or VS Code to view the step-by-step analysis.