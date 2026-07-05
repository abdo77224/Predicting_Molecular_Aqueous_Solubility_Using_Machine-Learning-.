🧪 Predicting Molecular Aqueous Solubility Using Machine Learning
📖 Overview

This project aims to predict the aqueous solubility (logS) of organic molecules using Machine Learning techniques. Predicting molecular solubility is a crucial step in drug discovery, as it helps researchers identify promising compounds while reducing the need for expensive and time-consuming laboratory experiments.

The application allows users to enter a molecule in SMILES format and instantly obtain its predicted aqueous solubility through an interactive Streamlit interface.

🚀 Features
✅ Molecular solubility prediction (logS)
✅ SMILES validation using RDKit
✅ Molecular descriptor extraction
✅ Morgan Fingerprint generation
✅ Feature selection and preprocessing
✅ Machine Learning model prediction
✅ Interactive Streamlit web application
📂 Dataset

The project uses the Delaney (ESOL) Dataset, which contains experimental aqueous solubility values for organic molecules.

Dataset size: 9,982 molecules
Target variable: logS (aqueous solubility)
⚙️ Workflow
SMILES
      │
      ▼
SMILES Validation (RDKit)
      │
      ▼
Molecular Descriptors
      │
      ▼
Morgan Fingerprints
      │
      ▼
Feature Selection
      │
      ▼
Data Standardization
      │
      ▼
Machine Learning Model
      │
      ▼
Predicted logS
🤖 Machine Learning Models

The following regression models were evaluated:

Linear Regression
Random Forest
Support Vector Regression (SVR)
XGBoost

Among these models, XGBoost achieved the best overall performance and was selected for deployment.

🛠️ Technologies Used
Python
Streamlit
RDKit
Scikit-learn
XGBoost
Pandas
NumPy
Joblib
📊 Evaluation Metrics

The models were evaluated using:

R² Score
Mean Absolute Error (MAE)
Root Mean Squared Error (RMSE)
K-Fold Cross Validation
💻 Installation

Clone the repository

git clone https://github.com/your-username/your-repository.git

Go to the project folder

cd your-repository

Install dependencies

pip install -r requirements.txt

Run the application

streamlit run app.py
