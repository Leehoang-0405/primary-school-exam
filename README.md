# Early Intervention Analytics: Predicting Academic Underperformance in Primary Education

## 1. Executive Summary
The primary education sector recognizes the critical importance of early literacy and numeracy skills. This project aims to address the sharp rise in student at risk of underperforming in the Year 3 NAPLAN writing test, which has increased by 87.7% from 2016 to 2021. 

Using the data collected by 40 schools across Australia and provided by Data2Intel, the following insights were extracted:
- SES background decreased slightly from Year 1 (102.94) to Year 2 (102.12).
- Students who perform well in literacy generally do well in numeracy and are less likely at risk of underperforming.
- Better vocabulary skills in Year 1 lower the risk of underperforming in the Year 3 writing test.
- Non-disabled students are less likely be at risk of underperforming compared to cognitively disabled students.


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

## 6. Model Integrity & Risk Assessment
A post-implementation audit of the predictive solution identifies the following strategic limitations:
* **Predictive Skew:** The current model relies heavily on literacy-oriented assessments. There is a risk of under-identifying students whose primary academic risks are rooted in numeracy or non-verbal reasoning.
* **Sample Specificity:** With 2000 records, the model is highly optimized for the current cohort. The predictive power may degrade when applied to schools with significantly different socio-economic (SES) profiles.
* **Operational Latency:** The reliance on Start-of-Year and End-of-Year snapshots provides point-in-time risk scores, which may miss rapid shifts in a student's academic trajectory during the term.
* **Static Evaluation:** Prioritizing Recall over Precision is effective for intervention, but the lack of a dynamic threshold means the model does not yet account for the shifting "cost of intervention" based on school resource cycles.

## 7. Next Steps
* **Multi-Dimensional Feature Integration:** Broaden the dataset to include a balanced mix of numeracy-based indicators and socio-demographic factors to create a "Whole-of-Child" risk profile.
* **Establishment of Feedback Loops:** Implement multiway communication between Data2Intel and educators to ensure the model aligns with real-world results and incorporates teacher feedback into future training sets.
* **Dynamic Threshold Tooling:** Develop a decision-support interface that allows administrators to adjust Recall/Precision targets based on current teacher availability and intervention capacity.
* **Model Generalisability Expansion:** Scale the dataset to include more diverse student populations to validate the model's performance across regional and metropolitan school districts.

## 8. Context and Credits
* **Client:** Data2Intel (Australian learning analytics consulting service). Client's name was anonymised due to confidentiality clause. 
* **Lead Analyst:** Lee Hoang.
* **AI Disclosure:** Generative AI was used to assist in the refinement of code and formatting within the original reports.
