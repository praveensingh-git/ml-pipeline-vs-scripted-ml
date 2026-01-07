
# `Pipeline()` vs No Pipeline 
### With and Without Scikit-learn Pipelines

## Overview
This repository contains **two production-oriented Machine Learning projects** built to demonstrate **best practices vs traditional workflows** in ML development.  
Both projects solve the same prediction problem but differ in **design philosophy, scalability, and deployment readiness**.

---

## Repository Structure

```
├── titanic_without_pipeline/
│   ├── titanic_without_pipeline.ipynb
│   └──titanic.csv
│   
│
├── titanic_pipelined/
│   ├── titanic_pipelined.ipynb ()
│   ├── titanic_data.csv (dataset)
│   └── prediction_with_pipeline.ipynb (saved model)
│   
└── README.md
```

---

## Project 1: ML Prediction Without Pipeline

### Objective
Build a machine learning model using a **traditional step-by-step approach**, handling preprocessing and modeling manually.

### Technical Workflow
1. Data ingestion using Pandas  
2. Exploratory Data Analysis (EDA)  
3. Missing value handling  
4. Categorical encoding  
5. Feature scaling  
6. Model training  
7. Prediction and evaluation  

---

## Project 2: ML Prediction With Scikit-learn `Pipeline()`

### Objective
Build a **production-ready ML system** using Scikit-learn Pipelines to encapsulate preprocessing and modeling.

### Technical Workflow
- Column-wise preprocessing using `ColumnTransformer`
- Numerical feature scaling via `StandardScaler`
- Categorical encoding via `OneHotEncoder`
- Model training integrated inside pipeline
- Unified `fit()` and `predict()` workflow

### Key Characteristics
- End-to-end automation
- Single source of truth for transformations
- Consistent train-test behavior

### Technical Advantages
- Prevents data leakage
- Clean and modular code
- Easy hyperparameter tuning
- Seamless deployment

---

## Technology Stack

- Python
- Pandas
- NumPy
- Scikit-learn
- Jupyter Notebook

---

## Comparison Summary

| Aspect | Without Pipeline | With Pipeline |
|------|------------------|---------------|
| Code Maintainability | Low | High |
| Data Leakage Safety | No | Yes |
| Deployment Ready | No | Yes |
| Feature Scalability | Poor | Excellent |
| Industry Standards | Basic | Professional |

---


⭐ If this project helped you evaluate ML best practices, consider starring the repository.
