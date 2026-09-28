# Customer Churn Analysis and Prediction Using Data Analytics and AI

## IBM SkillsBuild Data Analytics with AI Academic Internship Project

### Project Overview
This project analyzes customer churn for a fictional telecommunications company using the IBM Telco Customer Churn sample dataset. The workflow covers data cleaning, exploratory data analysis (EDA), visualization, feature preprocessing, machine-learning classification, model evaluation, model interpretation, and customer churn-risk scoring.

### Problem Statement
Customer churn can affect revenue and long-term customer relationships. The objective of this project is to understand customer characteristics associated with churn and build a model that estimates the probability that a customer will churn.

### Objectives
1. Load and inspect the customer dataset.
2. Clean missing and inconsistent values.
3. Explore churn patterns using statistical summaries and visualizations.
4. Prepare categorical and numerical variables for machine learning.
5. Train Logistic Regression and Random Forest classification models.
6. Compare model performance using Accuracy, Precision, Recall, F1-score, and ROC-AUC.
7. Interpret important model features.
8. Produce a customer-level churn-risk file.

### Dataset
**Dataset:** IBM Telco Customer Churn sample dataset  
**Records:** 7,043 customers  
**Original variables:** 21  
**Target:** `Churn`

**Dataset source:**  
https://raw.githubusercontent.com/IBM/telco-customer-churn-on-icp4d/master/data/Telco-Customer-Churn.csv

IBM's sample-data documentation describes Telco customer churn as a sample dataset for a fictional telecommunications company.

### Technologies Used
- Python
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Machine Learning

### Project Files
- `kudupudiGayathri _CustomerChurnAnalysis.ipynb` — complete project code and analysis.
- `requirements.txt` — Python dependencies.
- `kudupudi Gayathri _CustomerChurnAnalysisReport.docx` — project report.
- `README.md` — project overview and instructions.

The notebook also creates:
- `data/Telco-Customer-Churn.csv` — downloaded dataset.
- `customer_churn_risk_predictions.csv` — customer-level model predictions.

### Setup Instructions

#### 1. Install Python
Use Python 3.9 or newer.

#### 2. Install dependencies
Open a terminal in the project folder and run:

```bash
pip install -r requirements.txt
```

#### 3. Open Jupyter Notebook
Run:

```bash
jupyter notebook
```

Open:

`kudupudi Gayathri _CustomerChurnAnalysis.ipynb`

#### 4. Run the notebook
Run all cells from top to bottom.

The notebook automatically downloads the dataset if it is not already available in the `data` folder.

### Google Colab
1. Upload `YourName_CustomerChurnAnalysis.ipynb` to Google Colab.
2. Run the cells from top to bottom.
3. The notebook will download the dataset automatically if internet access is available.

### Model Evaluation
The notebook evaluates the models using:
- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC
- Confusion Matrix
- ROC Curve

The model with the highest test-set ROC-AUC is selected for the risk-scoring demonstration.

### Risk Scoring
The selected model estimates churn probability for each customer. Customers are grouped into:
- **Low risk:** probability below 0.30
- **Medium risk:** 0.30 to 0.60
- **High risk:** above 0.60

These bands are analytical thresholds chosen for demonstration and are not guarantees of future customer behavior.

### Important Limitations
- The dataset is a sample dataset for a fictional telecommunications company.
- It is a cross-sectional snapshot rather than a sequence of monthly observations.
- Predictive associations do not prove causation.
- Model performance can change on new or real-world data.
- Before operational use, the model should be validated, calibrated, monitored, and reviewed for fairness and business impact.

### Author
**Name:** kudupudi Gayathri  
**Program:** IBM SkillsBuild Data Analytics with AI Academic Internship  
**Organization:** BharatCares in association with AICTE
