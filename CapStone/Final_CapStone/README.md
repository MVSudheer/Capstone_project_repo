### Diabetes Risk Prediction Using Machine Learning – Final Report

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
This project utilizes a classification-based machine learning approach, as the objective is to predict whether a patient is likely to have diabetes or not. The outcome variable is binary in nature:

· 0 = non-diabetic

· 1 = Diabetic

Therefore, the expected output of the selected models is a categorical prediction indicating diabetes risk status. In addition to the predicted class label, some models (such as Logistic Regression) also provide probability scores, which can be interpreted as the likelihood of a patient being diabetic.

These probability estimates are valuable in healthcare settings because they allow practitioners to assess risk levels rather than relying solely on a binary decision.

The learning approach used in this project is supervised learning, as the dataset includes labeled outcomes (diabetes diagnosis) that guide the training process. The models learn patterns from historical patient data and use these patterns to predict outcomes for new, unseen cases.

The following supervised classification algorithms were implemented and compared:

· Logistic Regression (baseline model)

· Decision Tree

· Random Forest

· Support Vector Machine (SVM)

These models were selected to compare linear and nonlinear decision boundaries, interpretability, and predictive performance.

The primary goal of the predictive model is to accurately classify high-risk individuals while minimizing false negatives, as misclassifying diabetic patients could delay necessary medical intervention.

#### Results
What did your research find?
After evaluating all four models using accuracy, classification reports, and confusion matrices, Logistic Regression was selected as the optimal model.

Reasons for selection:

· Competitive accuracy performance

· Strong recall for diabetic class (medically critical)

· Balanced precision and F1-score

· Lower misclassification of positive (diabetic) cases

· High interpretability, which is essential in healthcare applications

Although ensemble models performed competitively, Logistic Regression provided the best combination of performance, stability, and interpretability for this diabetes prediction problem.

#### Next steps
What suggestions do you have for next steps?
To improve and extend this analysis, the following steps are recommended:

Implement additional models such as Decision Tree, Random Forest, and Support Vector Machine for performance comparison.
Translate model results into simple visual dashboards for non-technical stakeholders.

These next steps will strengthen the predictive accuracy and enhance the communication of insights for practical healthcare decision-making.

#### Outline of project

- [Link to notebook 1](CapStone/Final_CapStone/Final_capstone_project.ipynb)
- [Link to Final Project Report] (CapStone/Final_CapStone/Diabetes Risk Prediction Using Machine Learning Final Report.docx)
- [Link to Data files] (CapStone/Final_CapStone/Data)


##### Contact and Further Information