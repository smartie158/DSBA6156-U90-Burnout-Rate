# Stress Detection/ Burnout Rate: Are Your Employees Burning Out? 

### This is our DSBA 6156 Applied Machine Learning Final Project. 

### 
Employee stress and burnout have become significant concerns in today’s workplace, affecting employee well-being, productivity, and organizational performance. Factors such as excessive workloads, mental fatigue, job responsibilities, and limited workplace flexibility can contribute to increased burnout. Understanding the relationship between these factors and employee burnout can help organizations identify opportunities to improve workplace conditions and support employee well being.
The purpose of this project is to use machine learning to predict employee burnout levels and identify the factors most strongly associated with burnout. By analyzing employee characteristics, workload allocation, mental fatigue, and work-from-home availability, we aim to develop a predictive model that can help organizations recognize employees who may be experiencing elevated levels of burnout.
The primary machine learning task will be supervised regression, since the target variable, Burn Rate, is a continuous numerical value ranging from 0 to 1. A higher value represents a greater level of burnout.
Our project will address the following research questions:
Can machine learning accurately predict employee burnout levels using workplace and individual characteristics?
Which factors have the strongest relationship with employee burnout?
How do workload allocation, mental fatigue, and work-from-home availability relate to burnout levels?
How could these findings help organizations identify potential strategies for reducing employee stress and preventing burnout?
Data Sources
The data sources for this project will utilize three datasets that examine employee burnout mental health, and the influence of workplace and lifestyle factors on psychological well being. Each dataset provides a different perspective on factors that may contribute to burnout, allowing for a broader analysis of the relationship between professional responsibilities, personal circumstances, and mental health. 
The first dataset focuses on employee burnout and includes variables such as Employee ID, Data of Joining, Gender, Company Type, WFH (Work From Home) Setting, Designation, Resource Allocation, Mental Fatigue Score and Burn Rate. 
The second dataset provides information on demographics, lifestyle factors, mental health metrics, medical history, and coping strategies. Additional variables, including Financial Stress, Work Stress, and Self Esteem, will examine how personal and external stressors may influence an individual’s mental health. 
The third dataset is synthetically generated and includes demographic information, work conditions, lifestyle habits, social support, and psychological symptoms. This dataset will provide an additional opportunity to explore relationships between workplace environments, personal habits, and mental health outcomes. 
Features (Independent Variables) 
The independent variables will be selected based on their potential relationship with employee burnout and mental health outcomes. These features will include demographic characteristics, workplace conditions, lifestyle habits, psychological indicators, and social support factors. 
Workplace related features, such as resource allocation, work from home arrangements, designation, and work stress, will be examined to determine how professional responsibilities and working environments may contribute to burnout. Lifestyle and personal factors, including coping strategies, financial stress, self esteem and social support, will also be considered to better understand how external and psychological factors relate to employee well being. 
Target Variable (Dependent Variable) 
The primary target variable will be Burn Rate, which represents the level of employee burnout in the first dataset. The project will aim to identify which workplace, demographic, and psychological factors are most strongly associated with burnout and evaluate their predictive importance. 
For the remaining datasets, relevant mental health outcome variables will be evaluated as potential secondary targets, depending on their availability and how closely they align with the project’s research objectives. 
Proposed Data Preprocessing
Before developing the machine learning models, our team will clean and prepare the dataset using Python. We will identify missing values, duplicate records, unusual observations, and inconsistencies within the dataset. Records with missing target values will be excluded from supervised training, while missing numerical predictor values will be imputed using appropriate methods.
Categorical variables, including Gender, Company Type, and WFH Setup Available, will be converted into numerical representations using one-hot encoding. Numerical variables will be standardized when necessary, particularly for models sensitive to differences in feature scales. Employee ID will be excluded because it does not provide meaningful predictive information. We will also conduct exploratory data analysis using histograms, boxplots, scatterplots, and correlation analysis to better understand how workplace characteristics relate to burnout. Data will be divided into training and testing sets, with preprocessing methods fitted only on the training data to prevent data leakage.
Proposed Machine Learning Methodology
Our team will evaluate several supervised regression algorithms to predict employee burnout levels and determine which model provides the most accurate and reliable results.
Multiple Linear Regression: This model will establish a baseline for predicting employee burnout and help evaluate the direction and strength of relationships between workplace characteristics and burnout levels.
Decision Tree Regression: A Decision Tree will capture potential nonlinear relationships between employee characteristics and burnout. It will also provide interpretable decision rules to better understand which conditions are associated with higher burnout.
Random Forest Regression: Random Forest will combine multiple decision trees to improve predictive performance and reduce overfitting. Feature importance analysis will help identify the workplace characteristics most strongly associated with burnout.
Gradient Boosting Regression: Gradient Boosting will be used to determine whether sequentially improving predictions can provide greater accuracy than the other regression models.
The project will be completed using Python, primarily with Pandas, NumPy, Scikit-learn, Matplotlib, and Seaborn. Our team will conduct exploratory data analysis, preprocessing, model development, hyperparameter tuning, and model comparison.
An 80/20 training and testing split will be used, with five-fold cross-validation performed on the training data to support model selection. The final models will be evaluated using the held-out testing dataset.

