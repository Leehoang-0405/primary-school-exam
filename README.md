# Early Intervention Analytics: Predicting Academic Underperformance in Primary Education

## 1. Executive Summary
The primary education sector recognizes the critical importance of early literacy and numeracy skills. This project provides a machine learning solution for Data2Intel to identify students at risk of underperformance in the Year 3 Writing assessment. By identifying that 60% of students in the current cohort are at risk, this work enables proactive intervention strategies. The solution converts raw student data into actionable insights, allowing educators to provide support before learning disparities increase.

## 2. Business Problem
**The Decision:** Educators and stakeholders must decide which students require additional resources and literacy support during Year 1 and Year 2.

**The Failure:** Missing at-risk students can have detrimental long term effects on academic success. Relying on late-stage assessments increases learning disparities and possibly influences future studies. Without a predictive framework, the organization risks neglecting students who need prompt assistance.

**The Impact:** Failing to identify at-risk students early leads to a higher cost of intervention later in the academic lifecycle. This project shifts the focus from reactive reporting to proactive student support.

## 3. Methodology
* **Data Preparation and EDA:** Performed univariate and bivariate analysis on 2000 student records to identify key performance drivers.
* **Feature Engineering:** Executed data conversion by transforming categorical variables into dummy variables and handling missing values to ensure model readiness.
* **Predictive Modeling:** Developed and evaluated supervised machine learning models, specifically Logistic Regression and K-Nearest Neighbors (K-NN).
* **Evaluation Strategy:** Prioritised recall over precision to ensure that the maximum number of at-risk students are identified for early intervention.

## 4. Demonstration of Skills and Capabilities
* **Data Driven Feature Selection:** Identified that literacy oriented assessments generally have a stronger predictive effect against the target feature than numeracy oriented assessments.
* **Statistical Logic:** Utilised Logistic Regression to determine the odds of underperformance. Visualised coefficients to prove how specific early-year tests influence future results.
* **Optimisation for Impact:** Determined the best threshold based on F1 scores for both Logistic Regression and K-NN models to balance the costs of misclassification.
* **Technical Literacy:** Handled complex variables including disability status, SES background, and various reading assessments (Burt, Clay, and Text Reading) to build a multidimensional view of student risk.

## 5. Results and Business Recommendations
* **Impact:** The analysis proves that for every one-point increase in Burt-01-EOY scores, the odds of a student being at risk are reduced by 24.4%. 
* **Targeted Intervention:** A one-point increase in TextLevel-02-EOY reduces the odds of being at risk by 22.3%. 
* **Strategic Focus:** The model recommends that educators focus on improving skills in Burt-01-EOY and TextLevel-02-EOY to achieve better results and a lower chance of underperformance in the Year 3 NAPLAN writing test.
* **Value Delivery:** By using this predictive model, the organization can assist students who need support from a teacher while minimizing the long term cost of academic failure.

## 6. Next Steps
* **Model Generalisability:** Expand the dataset and include more diverse student populations to improve future predictions.
* **Feedback Loops:** Establish multiway communication between Data2Intel, business analysts, and educators to ensure the model aligns with real-world results.
* **Feature Refinement:** Consider excluding unrelated features with low correlation values, such as sibling order, to increase model efficiency.

## 7. Context and Credits
* **Client:** Data2Intel (Australian learning analytics consulting service).
* **Program:** MIS710: Machine Learning in Business.
* **Team:** Ba Huy Hoang Le (s224309594).
* **AI Disclosure:** ChatGPT and Google Gemini were used to assist in the refinement of code and formatting within the original reports.

```
