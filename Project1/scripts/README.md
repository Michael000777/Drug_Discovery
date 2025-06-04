# QSAR Modeling for SARS-CoV 3C-like Proteinase (CHEMBL3927)

This project builds and evaluates Quantitative Structure–Activity Relationship (QSAR) models to predict the bioactivity of small molecules targeting the **SARS coronavirus 3C-like proteinase (3CLpro, CHEMBL3927)** — a key enzyme involved in viral replication and a high-value target for antiviral drug discovery.

## 🔍 Objective

To leverage publicly available compound data from the **ChEMBL database** to train predictive models that can identify promising inhibitors of 3CLpro. This proof-of-concept pipeline supports virtual screening, lead prioritization, and drug repurposing workflows.

---

## 📦 Features

- ✅ ChEMBL data extraction via `chembl_webresource_client`
- 🧪 Compound preprocessing using **RDKit** (molecular descriptors, SMILES handling)
- 🤖 QSAR modeling using **scikit-learn** (Random Forest, SVM, etc.)
- 📈 Model evaluation 
- 💡 Feature importance and exploratory visualizations
- 🧬 Target: **CHEMBL3927 – SARS coronavirus 3C-like proteinase**

---

## ⚙️ Tech Stack

- `Python 3.9+`
- `RDKit` for cheminformatics
- `Pandas`, `NumPy`, `scikit-learn` for data processing and ML
- `matplotlib`, `seaborn` for visualizations
- `chembl_webresource_client` for ChEMBL access

---

## 🧪 Dataset

- Bioactivity data retrieved from **ChEMBL (CHEMBL3927)**  
- Only compounds with `standard_type = IC50` and non-null values were included  
- Activity threshold (e.g., 1000 nM) used to binarize compounds as **active/inactive**
