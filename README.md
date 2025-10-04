Hydrodynamic Prediction using Machine Learning in Slurry Bubble Columns

This repository contains Python scripts, supporting datasets, and graphical user interfaces (GUIs) developed for predicting key **hydrodynamic parameters** in **slurry bubble column reactors (SBCs)**, namely:

- **Gas holdup (αg)**
- **Mass transfer coefficient (kLa)**
- **Bubble rise velocity (Ub)**
- **Bubble size (db)**

The models are trained and validated using both **literature data** and **experimental measurements**, offering insights into how different parameters influence reactor-scale hydrodynamics.

---

Features

- 📊 Data preprocessing and dimensional analysis  
- 🤖 Machine learning model training (Decision Tree, Random Forest, Gradient Boosting)  
- 🔍 Hyperparameter tuning and performance evaluation  
- 🧠 Explainability analysis using SHAP values  
- 💻 GUI interfaces for user-friendly predictions and visualization  
- 📈 Parity plots, error metrics (R², MAE), and validation reports  

---

Folder Description

| Folder | Description |
|---------|-------------|
| `gas_holdup/` | Prediction of gas holdup using literature and experimental data |
| `mass_transfer_coefficient/` | Modeling of kLa using machine learning algorithms |
| `bubble_rise_velocity/` | Prediction of bubble rise velocity from operating conditions |
| `bubble_size/` | Estimation of bubble size distribution |
| `shap_analysis/` | SHAP value analysis for model interpretability |
| `hyperparameter_tuning/` | Grid search and contour visualization of model tuning |
| `loso_validation/` | Leave-One-Study-Out (LOSO) validation for robustness testing |
| `requirements.txt` | Python dependencies required to run all scripts |
| `LICENSE` | Open-source license file |
| `README.md` | Repository documentation |

---

Model Overview

Each parameter module includes:
- A **Python script** for training and testing ML models  
- A **dataset (.xlsx)** for input-output variables  
- Optionally, a **Tkinter GUI** for real-time predictions  
- Scripts for **visualization** (parity plots, feature importance, SHAP values)  

The machine learning models rely on **dimensionless correlations** (Reynolds, Froude, Weber, Eötvös numbers, etc.) to ensure generalization across systems and scales.

---

Installation and Setup

Clone the Repository
Open your terminal (or Git Bash on Windows) and run:
```bash
git clone https://github.com/PraneetPM/P.git
cd P
