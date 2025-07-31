# primary-school-exam

# Machine Learning in Business: Predicting Student Writing Performance

## Overview
This project aims to leverage machine learning to identify primary school students at risk of underperforming in writing by analyzing their early literacy and numeracy skills. The initiative is part of a collaborative effort with Data2Intel, an Australian learning analytics consultancy, to enhance educational outcomes for primary school students.

## Objectives
1. **Analytical Insights**:
   - Explore the socio-economic (SES) backgrounds and literacy skills of students.
   - Analyze relationships between demographic factors, disability conditions, and academic performance.
   - Uncover additional insights to inform targeted interventions.

2. **Machine Learning Applications**:
   - Develop two predictive models to identify students at risk of underperforming in writing by Year 3.
   - Create a clustering model to group students with similar characteristics for intervention strategies.

## Dataset
The project utilizes a dataset of 2,000 primary school students from over 40 schools in Australia. Key attributes include:
- Reading and numeracy skills measured in Years 1 and 2.
- Demographic, familial, and disability-related information.
- Writing performance measured through NAPLAN results in Year 3.

**Dataset Details**:
- Name: `LA4Schools.csv`
- No missing values; records with incomplete information were removed.
- Data spans five years (2016–2020).

## Key Tasks
### 1. Exploratory Data Analysis (EDA)
- Analyze socio-economic backgrounds of students.
- Investigate literacy and numeracy skill progression.
- Examine relationships between student attributes and writing performance risks.
- Derive actionable insights for early interventions.

### 2. Machine Learning Models
#### Predictive Models
- Train and evaluate two supervised learning models to predict Year 3 writing performance.
- Compare model performances and recommend the best-fit solution.

#### Clustering Model
- Apply unsupervised learning to group students into meaningful clusters.
- Interpret clusters to derive actionable recommendations.

### 3. Reporting
- **Technical Report**: Present findings and machine learning solutions to Data2Intel's Director of Data and Insights.
- **Business Report**: Summarize insights and actionable recommendations for the Director of Education and Engagement.

## Deliverables
1. **Reports**:
   - Analytical Report (Part A): Detailed findings and technical insights.
   - Business Report (Part B): Key results and actionable recommendations for stakeholders.
2. **Code**:
   - Python Notebook with detailed comments for model deployment.
   - PDF export of the notebook.

## Tools and Techniques
- **Programming Language**: Python
- **Libraries**: Pandas, NumPy, Matplotlib, Scikit-learn, etc.
- **Machine Learning Models**:
  - Supervised: Logistic Regression, Random Forest, or similar algorithms.
  - Unsupervised: K-Means Clustering or similar.

## Ethical Considerations
- Data privacy and compliance with ethical standards.
- Mitigating biases in model predictions.
- Transparency in recommendations and decision-making processes.

## How to Use
1. Clone the repository:
   ```bash
   git clone https://github.com/your-repo-name.git
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Open and run the Python notebook:
   ```bash
   jupyter notebook
   ```

## Contributors
- **Author**: Hoang Lee  
  Master of Business Analytics, Deakin University.

## Acknowledgments
This project is developed as part of the unit **MIS710 - Machine Learning in Business** at Deakin University. Special thanks to Data2Intel and Associate Professor Lemai Nguyen for providing the dataset and assessment framework.

## License
This project is for academic and research purposes only. Commercial use is prohibited without prior permission.
