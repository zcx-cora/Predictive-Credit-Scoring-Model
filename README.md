# Credit Scoring Using Machine Learning with SHAP-based Feature Selection

This repository contains the full codebase for an MSc thesis project on developing interpretable and effective credit scoring models. It explores both traditional and advanced machine learning models under application and behavioral scoring scenarios, using SHAP values for enhanced model explainability.

## 📂 Project Structure

| File/Folder                             | Description |
|----------------------------------------|-------------|
| `0_DataTreatment.ipynb`                | version 1 of data cleaning and preprocessing |
| `0_DataTreatment_V0.ipynb`             | version 2 of data treatment |
| `1_EDA.ipynb`                          | Exploratory Data Analysis |
| `2_NewClient_BasicModel.ipynb`         | Baseline model for the application scoring task |
| `2_NewClient_ablation study.ipynb`     | Ablation study on new client features |
| `3_NewClient_Model_topK.ipynb`         | Top-K SHAP-based model for application scoring |
| `4_All_client_BasicModel.ipynb`        | Baseline model for the application task |
| `5_AllClient_topK.ipynb`               | Top-K SHAP-based model for all clients |
| `LCDataDictionary.xlsx`                | Variable descriptions for the Lending Club dataset |
| `README.md`                            | Project overview and usage instructions |

## 📊 Dataset

The dataset is derived from Lending Club data and can be accessed from the following Google Drive link:  
[Download Lending Club dataset (Google Drive)](https://drive.google.com/file/d/1QpqMrD6Xg2ggNqFlwXPdoEUIgsLNjTQZ/view)

The dataset includes a rich set of loan-level features suitable for both **application scoring** (pre-loan) and **behavioral scoring** (post-loan) tasks.

## 🧠 Models

The following machine learning models were implemented and evaluated:

- Logistic Regression
- Decision Tree
- Random Forest
- XGBoost
- Support Vector Machine (SVM)
- Neural Networks (MLP)

## 🔍 SHAP-based Analysis

To improve model transparency and feature selection, SHAP (SHapley Additive exPlanations) values were used to:

- Rank feature importance
- Select top-K features
- Evaluate robustness under feature constraints

## 📌 Scenarios

This project includes two key real-world scoring settings:

1. **Application Scoring** – Predict default risk for new clients using only pre-loan information.
2. **Behavioral Scoring** – Assess existing borrowers using post-loan behavior variables.

## ⚙️ Requirements

To run the notebooks, make sure you have the following Python libraries installed:

```bash
pandas
numpy
scikit-learn
xgboost
matplotlib
seaborn
shap
