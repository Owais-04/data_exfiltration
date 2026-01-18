# AI-Based Hybrid Behavioral Anomaly Detection for Data Exfiltration

## 📌 Project Overview
This project implements a **hybrid machine learning framework** to detect **data exfiltration attacks** in network traffic.  
The system combines **supervised learning** for known attacks and **unsupervised anomaly detection** for unknown, encrypted, and low‑and‑slow exfiltration behavior.

The primary goal is to build a **robust, generalizable, and low false‑positive detection system** suitable for real‑world network environments.

---

## 🎯 Key Objectives
- Detect **known data exfiltration attacks** using supervised ML models
- Identify **unknown / zero‑day attacks** using behavioral anomaly detection
- Handle **encrypted traffic** without payload inspection
- Capture **low‑and‑slow exfiltration** using time‑series modeling
- Improve reliability using **ensemble risk scoring**
- Validate robustness through **cross‑dataset generalization**

---

## 🧠 System Architecture
The system is divided into three main components:

1. **Supervised Detection**
   - Random Forest
   - XGBoost  
   Used for detecting known, labeled exfiltration patterns.

2. **Unsupervised Detection**
   - Isolation Forest
   - Autoencoder
   - LSTM Autoencoder  
   Used for detecting unknown, anomalous, encrypted, and slow exfiltration behavior.

3. **Hybrid Ensemble**
   - Combines supervised probability and anomaly scores
   - Produces a final risk score for decision making

---


## 📊 Datasets Used
- **CIC‑Bell DNS Exfiltration Dataset**  
  Used for training supervised and unsupervised models.
- **UNSW‑NB15 Dataset**  
  Used for cross‑dataset generalization and robustness testing.

*(Datasets are used only for experimentation and are not included in this repository.)*

---

## ⚙️ Technologies & Tools
- **Programming Language:** Python
- **Machine Learning:** scikit‑learn, XGBoost
- **Deep Learning:** TensorFlow, Keras
- **Models:** Random Forest, Isolation Forest, Autoencoders, LSTM
- **Data Processing:** Pandas, NumPy
- **Visualization:** Matplotlib, Seaborn
- **Development Environment:** Jupyter Notebook

---

## 🧪 Methodology
1. **Data Preprocessing**
   - Cleaning and normalization
   - Feature scaling

2. **Feature Engineering**
   - Flow‑level features
   - Behavioral and time‑series features

3. **Model Training**
   - Supervised models trained on labeled data
   - Unsupervised models trained on normal behavior

4. **Anomaly Scoring**
   - Individual anomaly scores computed
   - Scores normalized and combined

5. **Hybrid Risk Scoring**

6. **Evaluation**
- Accuracy, Precision, Recall, F1‑Score
- ROC‑AUC
- Cross‑dataset generalization testing

---

## 🚀 How to Run the Project
1. Clone the repository
2. Place datasets inside the `data/` folder
3. Run notebooks in the following order:
- `supervised/supervised_model.ipynb`
- `unsupervised/unsupervised_model.ipynb`
- `combine/combine_results.ipynb`
4. View final predictions and evaluation metrics

---

## 📈 Results
- Improved detection of **encrypted and low‑and‑slow exfiltration**
- Reduced false positives using ensemble scoring
- Demonstrated generalization across different datasets

---

## 🏁 Conclusion
This project demonstrates how combining **supervised and unsupervised learning** improves the detection of sophisticated data exfiltration attacks.  
The hybrid approach ensures better adaptability to real‑world network environments where labeled data is limited and attack patterns constantly evolve.

---



