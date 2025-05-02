# Telecom Fraud Detection

## 📌 Project Overview
This project aims to build a machine learning model for detecting fraudulent behavior in a telecommunication company. Using real or simulated customer usage data (e.g., call records, SMS, internet usage), we apply ensemble learning techniques to classify and prevent fraudulent activities.

---

## ❓ Problem Description
Telecom fraud leads to millions in revenue losses globally. The goal is to detect fraud in customer behavior using classification models. Due to the highly imbalanced nature of the problem (very few fraud cases), special care is taken in model evaluation and selection.

**Type**: Binary Classification  
**Target Variable**: `is_fraud` (1 = Fraud, 0 = Legitimate)

We aim to:
- Improve recall on fraudulent instances to avoid missed detections.
- Maintain reasonable precision to avoid false positives.

---

## 🗂️ Project Structure

```
telecom-fraud-detection/
├── data/                # Raw and processed data
│   ├── raw/
│   └── processed/
├── notebooks/           # Jupyter notebooks for EDA and modeling
│   ├── 01_eda.ipynb
│   └── 02_modeling.ipynb
├── src/                 # Python modules (functions, training, utils)
│   ├── data_prep.py
│   ├── train_model.py
│   ├── evaluate.py
│   └── utils.py
├── models/              # Saved models
├── reports/             # Visual reports and charts
│   └── figures/
├── requirements.txt     # Python dependencies
├── .gitignore
└── README.md
```

---

## ⚙️ Setup Instructions

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/telecom-fraud-detection.git
   cd telecom-fraud-detection
   ```

2. **Create a virtual environment**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Run Jupyter notebooks**
   ```bash
   jupyter notebook
   ```

---

## ✅ TODOs
- [ ] Load and explore dataset
- [ ] Feature engineering
- [ ] Train baseline model
- [ ] Evaluate ensemble models
- [ ] Add SHAP/interpretability
- [ ] Export final model
