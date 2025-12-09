# 🧠 Creditworthiness Prediction

This project aims to predict **loan creditworthiness** — whether a borrower is likely to fully repay or default — using multiple machine learning models. The goal is to support financial institutions in minimizing default risks while improving lending decisions.

---

## 📊 Project Overview

| Model | Purpose | Scaled Data | Key Metric |
|--------|----------|-------------|-------------|
| Logistic Regression | Baseline model | ✅ | Precision |
| K-Nearest Neighbors (KNN) | Compare with non-parametric model | ✅ | Precision |
| Decision Tree | Interpretability & variable importance | ❌ | Precision |
| Artificial Neural Network (ANN) | Deep learning approach | ✅ | F1-Score |

---

## 🧩 Methodology

1. **Data Preprocessing**
   - Handle missing values and duplicates  
   - Convert categorical variables  
   - Scale numerical features using `StandardScaler`

2. **Train-Test Split**
   - 70% training, 30% testing  
   - Stratified sampling for balanced target distribution

3. **Model Training**
   - Logistic Regression, KNN, Decision Tree, ANN  
   - Hyperparameter tuning (GridSearchCV for KNN, Decision Tree)

4. **Model Evaluation**
   - Precision, Recall, F1-Score  
   - Confusion Matrix  
   - ROC-AUC Curve

---

## 📈 Results & Insights

- **Best model:** KNN with precision ≈ `80%`
- The model effectively identifies potential defaulters with minimal false negatives.
- Increasing decision threshold improved risk prediction for Class 1 (Default).
- Business implication: banks can reduce loan losses by prioritizing applicants with higher predicted repayment probability.

---

## 🧠 Business Recommendation

- Integrate the model into the **loan application screening process**.
- Use threshold tuning to control risk exposure.
- Combine predictive results with customer segmentation for targeted interventions.

---

## 🧰 Tools & Libraries

`Python`, `scikit-learn`, `pandas`, `numpy`, `matplotlib`, `tensorflow`, `keras`

---

## 🗂️ Project Structure
```
creditworthiness-prediction/
│
├── data/ # Raw and processed data
├── notebooks/
│ └── creditworthiness_model.ipynb
├── models/ # Saved trained models
├── results/ # Charts, metrics, and confusion matrices
├── requirements.txt
├── README.md
└── LICENSE
```
---

## 📎 How to Run

```bash
# 1. Clone this repository
git clone https://github.com/bartan29/creditworthiness-prediction.git

# 2. Navigate to the folder
cd creditworthiness-prediction

# 3. Install dependencies
pip install -r requirements.txt

# 4. Run the Jupyter Notebook
jupyter notebook notebooks/creditworthiness_model.ipynb
```

---

## 👤 Author
Muhammad Akbar Tantu
- Master of Commerce in Business Analytics & Cyber Security, UNSW Sydney
- 📧 muhammadakbartantu@gmail.com
- 🔗 https://www.linkedin.com/in/akbartantu/

---

## 📜 License
This project is licensed under the MIT License — see the LICENSE
 file for details.
© 2025 Muhammad Akbar

