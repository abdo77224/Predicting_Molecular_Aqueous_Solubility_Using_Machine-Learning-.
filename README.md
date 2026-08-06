# 🧪 Predicting Molecular Aqueous Solubility Using Machine Learning

<p align="center">
  <img src="images/poster.png" width="900">
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.11-blue?logo=python">
  <img src="https://img.shields.io/badge/Streamlit-WebApp-red?logo=streamlit">
  <img src="https://img.shields.io/badge/XGBoost-Regression-success">
  <img src="https://img.shields.io/badge/RDKit-Cheminformatics-orange">
  <img src="https://img.shields.io/badge/License-MIT-green">
</p>

---

## 📌 Overview

Molecular aqueous solubility (**logS**) is one of the most important physicochemical properties in drug discovery and pharmaceutical research. Poor solubility can significantly affect the bioavailability and therapeutic effectiveness of drug candidates.

This project presents an end-to-end **Machine Learning pipeline** for predicting the aqueous solubility (**logS**) of organic molecules directly from their **SMILES** representation.

The developed application enables researchers and students to instantly estimate molecular solubility through an intuitive **Streamlit** interface.

---

## 🎯 Objectives

- Predict aqueous solubility (logS) of organic molecules.
- Reduce reliance on expensive laboratory experiments.
- Compare several Machine Learning algorithms.
- Build an interactive prediction application.
- Demonstrate the use of AI in cheminformatics.

---

# 📊 Dataset

**Dataset:** Delaney (ESOL)

The dataset contains experimental aqueous solubility values for **9,982 organic molecules**.

Target Variable:

- **logS (Aqueous Solubility)**

Input:

- SMILES representation

---

# ⚙️ Project Workflow

```text
             SMILES
                │
                ▼
      SMILES Validation
          (RDKit)
                │
                ▼
 Molecular Descriptor Extraction
                │
                ▼
 Morgan Fingerprints (ECFP)
                │
                ▼
 Feature Selection
                │
                ▼
 Standardization
                │
                ▼
 Train / Test Split
                │
                ▼
 Machine Learning Models
                │
                ▼
 Hyperparameter Optimization
                │
                ▼
 Performance Evaluation
                │
                ▼
 Streamlit Deployment
```

---

# 🧬 Molecular Feature Extraction

The project uses **RDKit** to extract molecular descriptors from SMILES.

Examples include:

- Molecular Weight
- MolLogP
- TPSA
- Number of Hydrogen Bond Donors
- Number of Hydrogen Bond Acceptors
- Rotatable Bonds
- Ring Count
- Heavy Atom Count

Additionally, **Morgan Fingerprints (ECFP)** are generated to capture structural information.

---

# 🤖 Machine Learning Models

The following regression models were evaluated:

| Model | Purpose |
|--------|----------|
| Linear Regression | Baseline model |
| Random Forest | Ensemble learning |
| Support Vector Regression (SVR) | Non-linear regression |
| XGBoost | Gradient Boosting |

After comparison, **XGBoost** was selected as the final model due to its superior predictive performance.

---

# 📈 Evaluation Metrics

Model performance was assessed using:

- R² Score
- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- 5-Fold Cross Validation

---

# 💻 Streamlit Application

The deployed application allows users to:

✅ Enter a SMILES molecule

✅ Validate the chemical structure

✅ Compute molecular descriptors

✅ Predict aqueous solubility (logS)

✅ Display Lipinski's Rule of Five

✅ Classify molecule solubility

---

# 🛠️ Technologies

| Category | Tools |
|-----------|------|
| Programming | Python |
| Cheminformatics | RDKit |
| Machine Learning | Scikit-learn |
| Boosting | XGBoost |
| Data Analysis | Pandas, NumPy |
| Deployment | Streamlit |
| Model Persistence | Joblib |

---

# 📂 Repository Structure

```text
.
├── data/
│   ├── Delaney.csv
│
├── models/
│   ├── xgboost_model.pkl
│   ├── scaler.pkl
│
├── notebooks/
│
├── app.py
├── requirements.txt
├── README.md
```

---

# 🚀 Installation

Clone the repository

```bash
git clone https://github.com/your-username/repository-name.git
```

Move into the project

```bash
cd repository-name
```

Install dependencies

```bash
pip install -r requirements.txt
```

Run the application

```bash
streamlit run app.py
```

---

# 📷 Screenshots

## Home Page

_Add application screenshot here._

---

## Prediction Page

_Add application screenshot here._

---

## Results

_Add prediction screenshot here._

---

# 👨‍💻 Authors

- **Abdessalam Safadi**


---

# 👨‍🏫 Supervisors

- **Prof. El Habib Ben Lahmar**


---

# 🎓 Academic Context

This project was developed as a **Final Year Project (PFE)** at

**Faculty of Sciences Ben M'Sik**

**Hassan II University of Casablanca**

Academic Year **2025–2026**

---

# ⭐ Support

If you found this project useful, consider giving it a ⭐ on GitHub.

It helps others discover the project and supports future development.

---

## 📬 Contact

**Abdessalam Safadi**

📧 abdessalam.safadi@etu.univh2c.ma

LinkedIn: https://www.linkedin.com/in/abdessalam-safadi-0b1478245/

