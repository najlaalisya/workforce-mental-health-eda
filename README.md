# Workplace Wellbeing Analytics: A Statistical Study of Employee Mental Health

## 📌 Project Overview
This project explores the intersection of professional productivity and psychological wellbeing using data from a workplace mental health assessment tool. The goal was to transform raw, fragmented survey data into actionable insights regarding **Anxiety (GAD-2)**, **Depression (PHQ-2)**, **Stress (DASS-21)**, and **Loneliness (UCLA-3)**.

The analysis focuses on how different work environments (Remote vs. On-site) and demographic factors influence mental health outcomes and self-reported job performance.

> **Note:** The data used in this repository is **synthetic**, generated to mirror the statistical properties and structure of a real-world internal dataset while maintaining privacy and confidentiality.

---

## 🛠️ Data Engineering & Reconciliation
One of the primary challenges of this project was reconciling raw, nested survey data into a format suitable for clinical analysis.

* **Clinical Scoring**: Converted categorical survey responses into numerical indices based on standardized psychometric scales.
* **Data Normalization**: Cleaned and mapped inconsistent geographic data (e.g., mapping ISO country codes like `MY` or `ID` to full names) and demographic labels to ensure consistent grouping.
* **Feature Engineering**: Aggregated individual item scores to create "Risk Tiers" and "Impact Levels," allowing for high-level organizational health reporting.

---

## 🧩 Hypotheses & Analysis
The project follows a rigorous, hypothesis-driven Exploratory Data Analysis (EDA) approach using the following framework:

| Code | Hypothesis | Planned Analysis |
| :--- | :--- | :--- |
| **H1** | Poor mental health correlates with lower self-reported performance. | Spearman Correlation & Scatterplots |
| **H2** | Stress is a primary predictor of loneliness, independent of anxiety. | Multiple Linear Regression |
| **H3** | Remote work modes significantly alter loneliness scores compared to on-site roles. | Independent T-Tests / ANOVA |

---

## 📊 Key Insights
* **Productivity Correlation**: Analysis revealed that **Depression (PHQ-2)** scores had a more significant negative impact on self-reported workplace performance than **Anxiety (GAD-2)**.
* **The "Hybrid" Effect**: Employees in hybrid work models reported significantly lower loneliness levels than fully remote employees, despite reporting similar levels of daily stress.
* **Demographic Volatility**: Younger demographics (under age 25) showed higher volatility in stress scores, suggesting a need for targeted early-career support programs.

---

## 💻 Tech Stack
* **Language:** Python 3.10+
* **Data Manipulation:** `pandas`, `numpy`
* **Statistical Analysis:** `pingouin`, `statsmodels`, `scipy`
* **Visualization:** `seaborn`, `matplotlib`

---

## 🚀 How to Use
1.  **Clone the Repo**: 
    ```bash
    git clone [https://github.com/najlaalisya/wellbeing-analytics.git](https://github.com/najlaalisya/wellbeing-analytics.git)
    ```
2.  **Install Dependencies**:
    ```bash
    pip install pandas numpy pingouin seaborn statsmodels scipy
    ```
3.  **Run the Notebook**: Open the `.ipynb` file in Jupyter or VS Code to view the full pipeline from data cleaning to statistical inference.

---

## 📬 Contact
Created by [Najla Alisya] – feel free to reach out via [linkedin.com/in/najla-alisya]!
