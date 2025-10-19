# Credit-Risk-Modeling-with-Machine-Learning-in-Python
Here is a detailed and improved README file for your forked Credit Risk Modeling project, incorporating the core content and structure from the original while making it unique, professional, and comprehensive:

***

# Credit Risk Modeling with Machine Learning in Python

## Table of Contents

- [Background](#background)  
- [Project Overview](#project-overview)  
- [Modeling Pipeline](#modeling-pipeline)  
- [Key Documents and Notebooks](#key-documents-and-notebooks)  
- [Datasets](#datasets)  
- [Model Performance](#model-performance)  
- [Deliverables](#deliverables)  
- [Technologies Used](#technologies-used)  
- [Repository Structure](#repository-structure)  
- [Getting Started](#getting-started)  
- [Author](#author)  

***

## Background

Credit risk modeling is a fundamental aspect for financial institutions in understanding the risk of borrowers defaulting on loans or credit obligations. Borrowers may repay loans fully, partially, or default, potentially impacting the lender’s financial stability. Leveraging both statistical and advanced machine learning methods, this project builds models to accurately predict credit risk and ensure regulatory compliance.

***

## Project Overview

This project focuses on developing AI-powered credit risk models aligned with Basel II and Basel III regulatory frameworks. It aims to deliver a practical credit risk scorecard and a robust pipeline for calculating exposure loss metrics daily, enhancing decision-making for lenders.

***

## Modeling Pipeline

The credit risk assessment pipeline follows these stages:

1. **Data Preprocessing**  
   - Conversion of categorical attributes into dummy variables via fine and coarse classing.
2. **Probability of Default (PD) Modeling**  
   - Logistic regression to model and predict the likelihood of a borrower defaulting.
3. **Scorecard Creation**  
   - Generation of a credit scorecard reflecting the PD model results, designed for easy practical use.
4. **Loss Given Default (LGD) Modeling**  
   - Beta regression predicting the percentage of loss if default occurs.
5. **Exposure at Default (EAD) Modeling**  
   - Linear regression to estimate the outstanding loan amount at the time of default.
6. **Expected Loss (EL) Calculation**  
   - Integration of PD, LGD, and EAD to calculate expected losses.
7. **Model Monitoring**  
   - Validation with recent datasets to check population stability index and model robustness.

***

## Key Documents and Notebooks

- **L01 - Preprocessing and Feature Engineering**  
- **L02 - PD Modeling, Scorecard Development, and Cutoff Analysis**  
- **L03 - LGD, EAD, and EL Modeling**  
- **L04 - Population Stability Index & Model Validation**

***

## Datasets

The dataset is sourced from Lending Club, a large peer-to-peer lending platform in the US, containing over 800,000 consumer loans issued from 2007-2015. The data is split into historical (2007-2014) and recent (2015) for model training and validation to monitor predictive consistency over time.

***

## Model Performance

- **Probability of Default (PD)**  
  Model: Logistic Regression  
  Metrics: Accuracy 57.2%, ROC-AUC 0.684 (Above baseline 0.5)  
- **Loss Given Default (LGD)**  
  Stage 1: Logistic Regression (Accuracy 59.5%, ROC-AUC 0.64)  
  Stage 2: Linear Regression (Accuracy 77.7%)  
- **Exposure at Default (EAD)**  
  Model: Linear Regression (Accuracy 65.8%)  

Models demonstrate solid predictive performance with opportunities for further enhancement.

***

## Deliverables

- A practical and interpretable credit scorecard.  
- Dataframes to analyze the impact of cutoff rates on borrower acceptance.  
- Models for LGD, EAD, and EL computation.  
- Schema for monitoring population stability index for model drift detection.

***

## Technologies Used

- Python 3.8+  
- Jupyter Notebooks for modeling and visualization  
- Core libraries: pandas, numpy, scikit-learn, statsmodels, matplotlib, seaborn  
- Additional: beta-regression implementations, logistic regression, regression analysis

***

## Repository Structure

```
.
├── data/              # Raw and processed datasets  
├── notebooks/         # Jupyter notebooks for stepwise modeling  
├── src/               # Source code: preprocessing, modeling, evaluation scripts  
├── reports/           # Visualizations and generated reports  
├── requirements.txt   # Python dependency list  
├── LICENSE            # License file  
└── README.md          # Project documentation  
```

***

## Getting Started

1. Clone repository:  
   `git clone <https://github.com/rochitl72/Credit-Risk-Modeling-with-Machine-Learning-in-Python>`  
2. Install dependencies:  
   `pip install -r requirements.txt`  
3. Launch notebooks sequentially to run preprocessing, modeling, and evaluation.  
4. Replace datasets with your own for customization if desired.


***

## Author
Rochit Lenin  
***

