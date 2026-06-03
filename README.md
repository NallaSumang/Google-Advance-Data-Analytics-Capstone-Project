# HR Attrition Prediction: Data-Driven Suggestions for Salifort Motors

## Project Overview
This repository contains the capstone project for the Advanced Data Analytics program. The objective is to analyze a human resources dataset and build predictive models to uncover insights into employee turnover. By identifying the key factors that drive employees to leave, this project provides actionable, data-driven recommendations to improve employee retention.

## Objective
To design and build a predictive model (Machine Learning / Regression) that predicts whether an employee will leave the company based on their department, number of projects, working hours, evaluation scores, and satisfaction levels.

## Methodology: The PACE Framework
This project follows the **PACE** workflow:
* **Plan:** Define the business problem, stakeholder needs, and project scope.
* **Analyze:** Perform Exploratory Data Analysis (EDA) and data visualization to understand employee dynamics.
* **Construct:** Engineer features and train predictive models (Logistic Regression, Random Forest, etc.).
* **Execute:** Evaluate models, interpret feature importance, and deliver business recommendations.

## Files in this Repository
* `MAIN PROJECT FOR ADVANCE DATA ANALYTICS.ipynb`: The main Jupyter Notebook containing all the Python code, EDA, model training, and evaluation.
* `HR_capstone_dataset.csv`: The dataset used for model training. 
* `HR_Attrition_summary.pdf`: A one-page business summary of the findings intended for external stakeholders. 

## Tools & Libraries Used
* **Language:** Python
* **Data Manipulation:** Pandas, NumPy
* **Data Visualization:** Matplotlib, Seaborn
* **Machine Learning:** Scikit-Learn (Classification, Model Evaluation, Hyperparameter Tuning)

## Key Findings & Recommendations
### Conclusion, Recommendations, Next Steps

The models and the feature importances extracted from the models confirm that employees at the company are overworked. 

To retain employees, the following recommendations could be presented to the stakeholders:

* Cap the number of projects that employees can work on.
* Consider promoting employees who have been with the company for atleast four years, or conduct further investigation about why four-year tenured employees are so dissatisfied. 
* Either reward employees for working longer hours, or don't require them to do so. 
* If employees aren't familiar with the company's overtime pay policies, inform them about this. If the expectations around workload and time off aren't explicit, make them clear. 
* Hold company-wide and within-team discussions to understand and address the company work culture, across the board and in specific contexts. 
* High evaluation scores should not be reserved for employees who work 200+ hours per month. Consider a proportionate scale for rewarding employees who contribute more/put in more effort. 

**Next Steps**

It may be justified to still have some concern about data leakage. It could be prudent to consider how predictions change when `last_evaluation` is removed from the data. It's possible that evaluations aren't performed very frequently, in which case it would be useful to be able to predict employee retention without this feature. It's also possible that the evaluation score determines whether an employee leaves or stays, in which case it could be useful to pivot and try to predict performance score. The same could be said for satisfaction score. 

