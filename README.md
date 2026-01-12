# De-Novo-Drug-Design-with-Generative-AI-LSTM-
![Python](https://img.shields.io/badge/Python-3.8%2B-blue?style=flat&logo=python)
![TensorFlow](https://img.shields.io/badge/Deep_Learning-TensorFlow%2FKeras-orange?style=flat&logo=tensorflow)
![RDKit](https://img.shields.io/badge/Chemoinformatics-RDKit-green?style=flat)
![Status](https://img.shields.io/badge/Status-Research_Prototype-success
## 🛠️ Tech Stack
* **Language:** Python
* **Deep Learning:** TensorFlow / Keras
* **Chemoinformatics:** RDKit
* **Data Processing:** Pandas, NumPy
* **Visualization:** Matplotlib / RDKit Draw
## 📌 Project Overview
This project implements a **Generative Recurrent Neural Network (LSTM)** capable of designing novel, chemically valid molecular structures *de novo*. 
This AI approach acts throught learning the syntax of chemical language (SMILES) from the **ZINC database** to hallucinate new, synthetically accessible drug candidates.

The pipeline includes an automated ADMET screening system that filters generated molecules based on **Lipinski’s Rule of Five** and optimizes for high **QED (Quantitative Estimation of Drug-likeness)** scores.
## 🎯 Key Features
* **Generative AI Model:** A 2-layer LSTM network with Dropout layers to prevent overfitting.
* **Chemical Syntax Learning:** The model treats SMILES strings as a language, predicting atom-by-atom sequences.
* **Automated Screening Pipeline:**
    * **Validity Check:** RDKit parsing to ensure chemical stability.
    * **Lipinski’s Rule of Five:** Filters for bioavailability (MW < 500, LogP < 5).
    * **QED Metric:** Calculates *Quantitative Estimation of Drug-likeness* (0.0 - 1.0).

## 🧪 Results
The model successfully generates high-quality drug candidates. In the latest run, the model discovered molecules with **QED scores up to 0.92**.

**Generated Candidates (Filtered):**
<img width="900" height="900" alt="загружено (1)" src="https://github.com/user-attachments/assets/772ad1ff-c941-4843-8cb5-3172514e2e13" />

*Fig 1. De novo generated molecules with calculated Molecular Weight, LogP, and QED scores*



