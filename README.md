# Project Title: Analyzing School Learning Outcomes | Education Performance Insights 📚

Analyzing student performance data to identify key factors influencing **Math achievement**. The goal is to provide actionable recommendations for improving academic outcomes through data-driven strategies.

---

## Table of Contents
- <a href="#overview">Overview</a>
- <a href="#business-problem">Business Problem</a>
- <a href="#dataset-assumptions">Dataset & Assumptions</a>
- <a href="#tools-technologies">Tools & Technologies</a>
- <a href="#project-structure">Project Structure</a>
- <a href="#data-cleaning-preparation">Data Cleaning & Preparation</a>
- <a href="#exploratory-data-analysis-eda-key-insights">Exploratory Data Analysis (EDA) & Key Insights</a>
- <a href="#research-questions-answers">Research Questions & Answers</a>
- <a href="#final-recommendations">Final Recommendations</a>
- <a href="#future-work">Future Work</a>
- <a href="#how-to-run-this-project">How to Run this Project</a>
- <a href="#author-contact">Author & Contact</a>

---

<h2 id="overview">Overview</h2>

This project analyzes student-level education data to determine which school, teacher, and socio-economic factors most strongly impact **Math performance**. Using statistical analysis, visualizations, and a baseline Linear Regression model, the study provides **actionable insights and recommendations** to improve learning outcomes.
**🔗 Live Dashboard:**  
[Power BI Dashboard](https://app.powerbi.com/view?r=eyJrIjoiYjU1ZWQ4N2QtMmMzOC00ZTRlLThiMDktNGI0YTZmYTE4ZjJlIiwidCI6IjVjZTJiMzZmLTA0OTMtNGU5MC1hOWJjLThmNWFhYTc1OTQ2ZCJ9)
---

<h2 id="business-problem">Business Problem</h2>

The education sector requires **data-driven strategies** to allocate resources effectively and design targeted interventions.  

**Objective:**  
> Identify which school, teacher, and student-level variables are the strongest predictors of Math scores and suggest policies to enhance student achievement.

---

<h2 id="dataset-assumptions">Dataset & Assumptions</h2>

**Dataset Overview**
- 5200 student records
- 17 variables including:
  - Student performance (Math, Language, Science)
  - Teacher quality (Training, Experience, Teacher-Student Ratio)
  - School infrastructure (Internet, Electricity, Toilets, Library)
  - Socio-economic indicators
  - Geography & Demographics (Urban/Rural, District)

**Assumptions**
- Dataset is representative of the student population  
- Score percentages are standardized across schools  
- Binary infrastructure columns (1/0) accurately reflect resource availability  

---

<h2 id="tools-technologies">Tools & Technologies</h2>

**Programming:** Python  

**Libraries:**
| Library | Purpose |
|--------|---------|
| pandas | Data cleaning & manipulation |
| numpy | Numerical operations |
| matplotlib & seaborn | Visualization & statistical graphics |
| scikit-learn | Linear Regression modeling |

**Environment:** Jupyter Notebook

---

<h2 id="project-structure">Project Structure</h2>

| File Name | Description |
|-----------|-------------|
| School_data.csv | Raw dataset |
| cleaned_data_for_analysis.csv | Cleaned dataset for modeling |
| Analyzing_School_Learning_Outcomes.ipynb | Full analysis & visualizations |
| Project Report | Final compiled presentation |
| README.md | Project documentation |

---

<h2 id="data-cleaning-preparation">Data Cleaning & Preparation</h2>

| Step | Description | Status |
|------|-------------|--------|
| Duplicate check | No duplicate entries | ✅ |
| Outlier removal | Removed unrealistic Math scores (>100) and Parent Literacy outside 0–100 | ✅ |
| Missing values | Imputed using mean/mode | ✅ |
| Teacher_Student_Ratio | Corrected after filtering | ✅ |

**Final Data Status:**  
- Clean, standardized dataset ready for modeling  
- Adequate sample size maintained  

---

<h2 id="exploratory-data-analysis-eda-key-insights">Exploratory Data Analysis (EDA) & Key Insights</h2>

**Academic Relationships**
- Math & Language: r = 0.84 (very strong)  
- Math & Science: r = 0.78 (strong)  
- Dense score at 60% → likely passing threshold

**Teaching Factors**
- Teacher training improves student outcomes  
- Teacher experience shows minimal impact (r = -0.018)  
- Teacher-Student Ratio not impactful (r = 0.003)

**Infrastructure Factors**
- Schools with Library, Electricity, Internet → higher excellence rates  
- Internet availability is the single most influential factor  
- Schools lacking infrastructure have higher failure rates

**Urban vs Rural**
- Urban students consistently outperform rural students

---

<h2 id="research-questions-answers">Research Questions & Answers</h2>

| Research Question | Key Finding |
|------------------|-------------|
| What predicts Math performance best? | Language proficiency (r = 0.84) |
| Do teacher characteristics matter? | Training matters; Experience does not |
| Does infrastructure affect outcomes? | Yes — Internet & Electricity most impactful |
| Urban vs Rural gap? | Urban students perform better |

---

<h2 id="final-recommendations">Final Recommendations</h2>

1. **Increase Teacher Professional Development**  
   - Minimum of 6 high-quality trainings per teacher  

2. **Ensure Universal Infrastructure**  
   - Electricity + Internet for all schools  

3. **Integrate Literacy into Math Curriculum**  
   - Leverage strong Math-Language correlation (r = 0.84)

---

<h2 id="future-work">Future Work</h2>

- Explore advanced ML models (Random Forest, Gradient Boosting)  
- Include richer socio-economic features  
- Evaluate digital education initiatives  

---

<h2 id="how-to-run-this-project">How to Run this Project?</h2>

1.  **Clone the Repository:**
    ```bash
    git clone https://github.com/Shazmeengithub/Analyzing_School_Learning_Outcomes-Python-PowerBI
    ```
2.  **Install Dependencies:**
    ```bash
    # Install the libraries used in the code
    pip install pandas numpy matplotlib seaborn scikit-learn
    ```
3.  **Execute the Analysis:**
    * Open and run the `Analyzing_School_Learning_Outcomes.ipynb` file to execute the code and reproduce the analysis, visualizations, and insights.

---
<h2 id="author-contact">Author & Contact</h2>

* **Author:** Shazmeen Shaikh
* **Contact:** https://www.linkedin.com/in/shazmeen-shaikh-30bb63237/
