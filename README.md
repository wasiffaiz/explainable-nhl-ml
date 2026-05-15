[README.md](https://github.com/user-attachments/files/27813644/README.md)
# Explainable Machine Learning for Early Detection of Non-Hodgkin's Lymphoma

This repository contains an academic machine learning project focused on predicting a selected Non-Hodgkin's Lymphoma-related outcome using structured clinical data. The project combines predictive modelling with explainability and reliability analysis to support healthcare-oriented decision-support research.

> **Disclaimer:** This project is for academic and portfolio purposes only. It is not intended for real clinical diagnosis, treatment planning, or medical decision-making.

## Project Aim

The aim of this project is to build and evaluate an explainable machine learning pipeline that can predict a selected Non-Hodgkin's Lymphoma-related outcome while maintaining interpretability, robustness, and reliability.

## Tools and Technologies

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn
- SHAP
- Joblib

## Machine Learning Models

The project compares multiple supervised machine learning models:

- Random Forest
- Histogram Gradient Boosting
- Multi-Layer Perceptron (MLP)

## Key Results

- Final selected model: **Random Forest**
- Test ROC-AUC: **0.875**
- Default threshold: **0.50**
- Selected threshold: **0.35**
- Recall improved from **0.500** to **0.717** after threshold tuning
- SHAP explainability was used to identify influential clinical features

## Project Workflow

1. Data exploration
2. Data cleaning and preprocessing
3. Handling missing values and categorical variables
4. Leakage-prone feature removal
5. Model training and comparison
6. Model evaluation using accuracy, precision, recall, F1-score, ROC-AUC, Brier score, and calibration analysis
7. Threshold tuning for healthcare-oriented recall improvement
8. Cross-validation for model stability
9. Robustness testing under missing-data and imbalance conditions
10. SHAP, permutation importance, and partial dependence analysis for explainability

## Repository Structure

```text
explainable-nhl-ml/
|
|-- notebooks/
|   |-- 01_Data_Exploration.ipynb
|   |-- 02_Data_Preprocessing.ipynb
|   |-- 03_Model_Training.ipynb
|   |-- 04_Reliability_Robustness_Explainability.ipynb
|
|-- data/
|   |-- README.md
|
|-- results/
|   |-- README.md
|   |-- figures/
|
|-- models/
|   |-- README.md
|
|-- README.md
|-- requirements.txt
|-- .gitignore
```

## Notebooks

### 01_Data_Exploration.ipynb
Explores the raw clinical dataset, reviews missingness, checks feature structure, and identifies suitable target preparation steps.

### 02_Data_Preprocessing.ipynb
Handles data cleaning, train-validation-test splitting, categorical encoding, missing-value treatment, and reproducible preprocessing.

### 03_Model_Training.ipynb
Builds and compares machine learning models using consistent preprocessing and evaluates model performance.

### 04_Reliability_Robustness_Explainability.ipynb
Performs threshold tuning, cross-validation, calibration analysis, robustness testing, and SHAP-based explainability.

## How to Run

1. Clone the repository:

```bash
git clone https://github.com/YOUR_USERNAME/explainable-nhl-ml.git
cd explainable-nhl-ml
```

2. Create a virtual environment:

```bash
python -m venv .venv
```

3. Activate the virtual environment:

On Windows:

```bash
.venv\Scripts\activate
```

On macOS/Linux:

```bash
source .venv/bin/activate
```

4. Install dependencies:

```bash
pip install -r requirements.txt
```

5. Open Jupyter Notebook:

```bash
jupyter notebook
```

Then run the notebooks in order from `01` to `04`.

## Dataset Note

The dataset is not included in this repository. This is to keep the repository clean and avoid uploading unnecessary or sensitive data files. The project was developed using structured clinical data obtained from cBioPortal.

## Portfolio Summary

This project demonstrates skills in:

- Python programming
- Data preprocessing
- Exploratory data analysis
- Machine learning classification
- Model evaluation
- Threshold tuning
- Cross-validation
- Calibration analysis
- Robustness testing
- Explainable AI using SHAP
- Healthcare-oriented predictive modelling
