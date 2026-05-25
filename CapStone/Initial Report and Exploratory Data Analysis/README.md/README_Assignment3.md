### Exploratory Analysis and Predictive Modeling for Diabetes Detection

**Sudheer Manuri**

#### Executive summary
This project aims to predict whether a patient is at high risk of developing diabetes using demographic and clinical health indicators. Through exploratory data analysis and a baseline machine learning model, key risk factors were identified and evaluated for their predictive power. The findings demonstrate that structured patient health data can be used to support early detection efforts and assist healthcare providers in preventive decision-making.

#### Rationale
Why should anyone care about this question?
Diabetes is a chronic disease that often develops gradually and may remain undiagnosed until serious complications occur. Early identification of high-risk individuals can significantly reduce long-term health risks, treatment costs, and hospital burden.

If this question remains unanswered, healthcare systems may continue relying solely on traditional screening methods, which may not fully leverage available patient data. By using predictive analytics, healthcare providers can proactively identify at-risk patients and recommend early lifestyle or medical interventions. This can improve patient outcomes, reduce complications, and optimize healthcare resource allocation.

#### Research Question
What are you trying to answer?
Can demographic and clinical health indicators be used to accurately predict whether a patient is at high risk of developing diabetes?

#### Data Sources
What data will you use to answer you question?
The dataset used for this project is the Pima Indians Diabetes dataset, obtained from the Kaggle.

The dataset includes:

Patient demographics (age)
Clinical measurements (glucose level, blood pressure, BMI, insulin, skin thickness)
Pregnancy history
Diabetes pedigree function (family history indicator)
Outcome variable (diabetes diagnosis: positive or negative)

This dataset provides structured numerical features suitable for classification modeling.

#### Methodology
What methods are you using to answer the question?
The following steps were performed:

Data Cleaning
Identified invalid zero values in medical measurements.
Replaced invalid entries with median values.
Verified class distribution.

Exploratory Data Analysis (EDA)
Examined feature distributions.
Created visualizations to compare diabetic vs non-diabetic patients.
Conducted correlation analysis to identify strong predictors.

Feature Preparation
Separated independent variables and target variable.
Standardized numerical features.
Split the dataset into training and testing sets.

Baseline Model
Implemented Logistic Regression as a baseline classification model.
Evaluated model performance using accuracy and classification metrics.

This approach provides both statistical understanding and predictive modeling capability.

#### Results
What did your research find?
The exploratory data analysis and baseline Logistic Regression model produced several important findings.

First, the model achieved an overall accuracy of approximately 75%, indicating that patient demographic and clinical data can reasonably predict diabetes risk.

From the classification results:
The model performed stronger in identifying non-diabetic patients (higher precision and recall).
It showed moderate performance in identifying diabetic patients, with lower recall. This suggests that some high-risk individuals were misclassified as non-diabetic.
This is important because, in a healthcare context, failing to identify diabetic patients (false negatives) may have serious consequences.

Key Predictive Factors

Based on the model coefficients, the most influential predictors of diabetes risk were:
Glucose level (strongest positive predictor)
BMI
Age
Diabetes Pedigree Function (family history)
Number of pregnancies

These variables significantly increase the likelihood of diabetes when their values are higher.
Interestingly:
Blood Pressure and Insulin showed negative coefficients in the model.
Skin Thickness had only a small impact.

Overall, the research confirms that glucose level, body mass index, age, and family history are strong indicators of diabetes risk. The baseline model demonstrates meaningful predictive capability, though improvements may be needed to better detect high-risk patients.

#### Next steps
What suggestions do you have for next steps?
To improve and extend this analysis, the following steps are recommended:

Implement additional models such as Decision Tree, Random Forest, and Support Vector Machine for performance comparison.
Translate model results into simple visual dashboards for non-technical stakeholders.

These next steps will strengthen the predictive accuracy and enhance the communication of insights for practical healthcare decision-making.

#### Outline of project

- [Link to notebook 1]()
- [Link to notebook 2]()
- [Link to notebook 3]()


##### Contact and Further Information