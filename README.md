Employee Attrition Prediction System
Problem Statement
Employee attrition can lead to increased recruitment costs, productivity loss, and knowledge gaps within an organization. This project uses machine learning to predict employee attrition and identify the key factors that contribute to employee turnover, enabling HR teams to take proactive retention measures.

Dataset
Name: IBM HR Analytics Employee Attrition & Performance Dataset
Source: IBM HR Analytics Dataset
Link: https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset
Rows / Columns: 1,470 rows, 35 columns (32 columns after removing constant features)
Tools Used
Python
Pandas
NumPy
Matplotlib
Seaborn
Scikit-learn
StandardScaler
Logistic Regression
Decision Tree Classifier
Random Forest Classifier
Workflow
Data Collection
Data Cleaning
Exploratory Data Analysis (EDA)
Feature Encoding
Train-Test Split
Feature Scaling
Model Building
Logistic Regression
Decision Tree
Random Forest
Model Evaluation
Feature Importance Analysis
Business Recommendations
Results
Model Comparison
Model	Accuracy	Precision	Recall	F1-Score
Logistic Regression	56.46%	21.17%	59.18%	31.18%
Decision Tree	28.23%	15.09%	71.43%	24.91%
Random Forest	83.33%	0.00%	0.00%	0.00%
Recommended Model
Logistic Regression

Although Random Forest achieved the highest overall accuracy (83.33%), it failed to identify any employees who actually left the company, resulting in zero recall for attrition cases. Logistic Regression provided the best balance between identifying at-risk employees and maintaining overall model stability, making it the most suitable model for employee retention initiatives.

Top Factors / Drivers
Work-Life Balance

Employees reporting poor work-life balance showed a higher likelihood of attrition.
Monthly Income

Lower monthly income levels were associated with increased employee turnover risk.
Total Working Years

Employees with fewer years of experience demonstrated higher attrition probabilities.
OverTime

Employees working overtime were more likely to leave the organization.
Job Role and Education Field

Certain job roles and education backgrounds showed higher attrition patterns than others.
Key Insights
Employee attrition is highly imbalanced, with approximately 16.5% of employees leaving the company.
Work-life balance and overtime emerged as important indicators of employee satisfaction and retention.
Salary-related variables consistently appeared among the strongest predictors across multiple models.
High accuracy alone can be misleading in imbalanced classification problems.
Recall is especially important in attrition prediction because failing to identify at-risk employees reduces the effectiveness of retention programs.
## Screenshots
Images/age_distribution_attrition.png
Images/monthly_income_attrition.png
Images/overtime_attrition.png
Images/jobrole_attrition.png
Images/feature_importance.png

## Business Recommendations
1. Improve Work-Life Balance
Implement flexible work arrangements, hybrid work options, and monitor employee workload to reduce burnout and voluntary turnover.

2. Reduce Excessive Overtime
Establish overtime thresholds and encourage managers to proactively address workload concerns before employees become disengaged.

3. Review Compensation Strategies
Conduct regular salary benchmarking and create retention-focused compensation plans for critical talent groups.

4. Develop Career Growth Programs
Create structured career advancement opportunities, mentorship programs, and training initiatives to improve employee engagement and long-term retention.

5. Build an Early-Warning Attrition Dashboard
Deploy the predictive model within an HR analytics dashboard to identify high-risk employees and support proactive intervention efforts.

Future Improvements
Address class imbalance using SMOTE or other oversampling techniques.
Tune Random Forest hyperparameters to improve minority-class prediction.
Explore advanced models such as XGBoost and LightGBM.
Evaluate models using ROC-AUC and Precision-Recall curves.
Deploy the solution as a Streamlit or Power BI dashboard for HR teams.
## Author
[Edwin Nkengafac] | [https://www.linkedin.com/in/edwin-nkengafac-27137a2b3/]
