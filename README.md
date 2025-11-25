# Smart Complaint Prioritizer 

![Python](https://img.shields.io/badge/Python-3.10%2B-blue)
![Status](https://img.shields.io/badge/Status-Data%20Engineering%20Complete-green)
![Library](https://img.shields.io/badge/Library-Pandas%20|%20VADER%20|%20ScikitLearn-orange)

An End-to-End Machine Learning project to classify Consumer Finance Complaints and predict their priority level using NLP.

## Project Goal
To build an automated pipeline that:
1.  **Ingests** massive government datasets (CFPB Consumer Complaints) via chunking.
2.  **Analyzes** text sentiment and severity using **VADER** and keyword logic.
3.  **Classifies** complaints into Priority Levels (High/Medium/Low).
4.  **Predicts** issue categories using ML (Random Forest/XGBoost).

## Project Structure
```text
smart-complaint-prioritizer/
├── data/                  # Gitignored (Raw data ~800MB)
├── notebooks/             # Jupyter Notebooks for experiments
│   ├── 01_data_collection.ipynb    # Chunked ingestion & filtering
│   ├── 02_feature_engineering.ipynb # VADER sentiment & Priority Logic
│   └── 03_eda.ipynb                # (In Progress) Visualizations
├── src/                   # Source scripts (modular code)
├── README.md              # Project documentation
└── requirements.txt       # Dependencies