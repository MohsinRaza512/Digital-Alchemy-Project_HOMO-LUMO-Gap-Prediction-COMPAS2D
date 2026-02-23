# Digital Alchemy Project
## HOMO-LUMO Gap Prediction from Molecular Structure  
### Comparative Machine Learning Study on COMPAS-2D Dataset  

## 📌 Project Overview
This project investigates whether the HOMO-LUMO gap of heteroaromatic molecules can be predicted from 2D molecular structure alone using machine learning models.

The study compares seven regression models under Murcko scaffold splitting to enforce structural generalisation.

## 🧪 Dataset
- COMPAS-2D dataset (52,000 neutral molecules used)
- DFT-computed HOMO-LUMO gaps
- Atoms: B, C, N, O, S

## ⚙️ Feature Engineering
- RDKit molecular descriptors (~200 features)
- 1024-bit Morgan fingerprints (radius=2)
- Total feature space: 1264 dimensions

## 🤖 Models Compared
- Linear Regression
- Ridge
- Lasso
- ElasticNet
- Random Forest
- Gradient Boosting
- XGBoost

## 🏆 Best Model
Gradient Boosting:
- R² = 0.752
- MAE = 0.266 eV
- Scaffold split evaluation

## 🔬 Key Findings
- Tree-based models outperform linear models due to nonlinear structure-property relationships.
- Boron atom count is a dominant predictor.
- Outlier analysis reveals prediction failures are linked to rare Morgan fingerprint fragments.

## 📂 Files
- `compas2d_final.ipynb` → Complete reproducible implementation
- `COMPAS_2D_Digital_Alchemy_Report_Template1 (3).pdf` → Final written report

## 🔁 Reproducibility
All seeds and hyperparameters are fixed in the notebook.

## 👤 Author
Mohsin Raza  
MSc Artificial Intelligence  
FAU Erlangen-Nürnberg
