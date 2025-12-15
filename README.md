# Salifort Motors: Employee Retention Project

![Status](https://img.shields.io/badge/Status-Complete-green)
![Python](https://img.shields.io/badge/Python-3.9-blue)
![Libraries](https://img.shields.io/badge/Libraries-Pandas%2C%20Scikit--Learn%2C%20XGBoost-orange)

## 📄 Project Overview
This project is the capstone for the **Google Advanced Data Analytics Professional Certificate**. 

**Salifort Motors**, a fictional large consulting firm, sought to reduce high employee turnover rates. The goal of this analysis was to identify the key factors contributing to employee attrition and build a predictive model to determine the likelihood of an employee leaving the company.

## 🎯 Business Understanding
The HR department collected data on 15,000 employees. The high cost of recruiting and training new employees makes retention a financial priority.
* **Stakeholders**: HR Department, Executive Leadership.
* **Goal**: Predict whether an employee will leave and offer strategies to improve retention.

## 📊 Data Understanding
The dataset contained 14,999 observations and 10 variables. Key features included:
* `satisfaction_level`: Self-reported satisfaction (0-1).
* `last_evaluation`: Score of last performance review (0-1).
* `number_project`: Number of projects assigned.
* `average_monthly_hours`: Average hours worked per month.
* `time_spend_company`: Years at the company.
* `left`: Target variable (1 = Left, 0 = Stayed).

## 🛠️ Methodology (PACE Framework)
This project followed the **PACE** (Plan, Analyze, Construct, Execute) workflow:
1.  **Plan**: Defined project scope and inspected data structure.
2.  **Analyze**: Conducted Exploratory Data Analysis (EDA) to visualize relationships between variables (e.g., turnover vs. hours worked).
3.  **Construct**: Built and tuned machine learning models (Logistic Regression, Decision Tree, Random Forest, XGBoost).
4.  **Execute**: Interpreted model results and formulated business recommendations.

## 🤖 Modeling and Evaluation
The **XGBoost** and **Random Forest** models performed best, achieving high accuracy and recall scores. The models identified `satisfaction_level`, `last_evaluation`, and `number_project` as the most influential features.

| Model | Precision | Recall | F1-Score | Accuracy |
|---------------------|-----------|--------|----------|----------|
| Logistic Regression | 44% | 27% | 33% | 82% |
| Decision Tree | 97% | 92% | 94% | 98% |
| Random Forest | 99% | 91% | 95% | 99% |
| XGBoost | 98% | 93% | 95% | 99% |

## 💡 Key Insights & Recommendations
Based on the analysis, the following factors drive turnover:
1.  **Overwork**: Employees working 250+ hours/month or assigned 7 projects are highly likely to leave.
2.  **The "4-Year Wall"**: Attrition peaks around the 4-year mark, suggesting a lack of advancement opportunities or burnout.
3.  **Performance Paradox**: High performers working long hours are leaving, likely due to burnout or lack of recognition relative to effort.

**Recommendations for Salifort Motors:**
* **Cap Workload**: Limit the number of projects to 3-4 per employee to prevent burnout.
* **Review Promotions**: Investigate why employees with 4+ years of tenure are leaving; implement clear career progression paths.
* **Compensation Review**: Ensure high-performing employees working overtime are adequately rewarded, rather than just assigning them more work.

## 📂 Project Structure
* `Salifort_Motors_Project.ipynb`: The full analysis and modeling code.
* `data/`: Contains the dataset used for analysis.
* `docs/`: Executive summary and presentation slides.
* `certificate/`: Proof of completion for the Google Advanced Data Analytics Certificate.

## 📜 License
This project is part of the Google Advanced Data Analytics Professional Certificate on Coursera.
