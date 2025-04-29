# Loan_Risk_Anlaysis

Project Goal: This project predicts loan approval risk by applying Principal Component Analysis (PCA) for dimensionality reduction, followed by Predictive Discriminant Analysis (LDA) and Random Forest Classifier for classification.
Models are evaluated based on Precision, Recall, F1 Score, Accuracy, and ROC AUC, with special focus on maximizing precision to avoid high-risk approvals.
Both models also undergo threshold adjustment to improve precision further. Principal components (PC2 and PC7) are interpreted to understand key factors influencing model decisions.

Folder Contents:

    -LoanRisk_Prediction.ipynb — Main Jupyter Notebook (full analysis)
    -loan_sanction_train.csv — Training dataset used
    -README.md — This file (instructions)


Installation and Requirements:

    You will need Python 3.7+ installed.
    Install required Python packages by running:
    pip install pandas numpy scikit-learn matplotlib
    Or if you use Jupyter Notebooks:
    conda install pandas numpy scikit-learn matplotlib


How To Run Project:

    -Clone or download this repository.
    -Place the loan_sanction_train.csv file in the same folder as the notebook.
    -Open and run the LoanRisk_Prediction.ipynb notebook sequentially.

Follow these sections inside the notebook:

    -Data Cleaning and Preparation
    -PCA Transformation (12 components)
    -LDA Training and Threshold Adjustment
    -Random Forest Training and Threshold Adjustment
    -Model Evaluation (Confusion Matrices, Precision, Recall, F1 Score, Accuracy, ROC AUC)
    -PCA Loadings Interpretation
    -Important Feature Analysis for PC2 and PC7
    
    Visualizations:
        -Scree Plot
        -ROC Curves
        -Precision-Recall Curves
        -Feature Importance Bar Charts


Outputs Generated:

    -Confusion matrices for both models
    -ROC-AUC and Precision-Recall curves
    -Scree plot for PCA
    -Bar charts showing model performance metrics
    -Bar charts showing top features contributing to important principal components



  Notes:

    -The models adjust the classification threshold to 0.65 instead of the default 0.5 to prioritize precision.
    -PCA is fitted before modeling, based on standardized feature scaling.
    -The project focuses on interpretability (via PCA loadings) as well as predictive performance.
