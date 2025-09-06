# 🫀 Heart Disease Prediction using Machine Learning

This project applies multiple **Machine Learning algorithms** to predict the likelihood of cardiovascular disease based on clinical attributes.  
It uses the **UCI Cleveland Heart Disease dataset** and compares models on **accuracy, precision, recall, and F1-score**.

---

## 📌 Project Overview
- **Goal:** Predict heart disease (target: 1 = disease, 0 = no disease).  
- **Dataset:** UCI Cleveland Heart Disease dataset .  
- **Models Implemented:**
  - K-Nearest Neighbors (KNN)
  - Logistic Regression
  - Support Vector Machine (SVM – RBF kernel)
  - Decision Tree
  - Random Forest  

- **Evaluation Metrics:** Accuracy, Precision, Recall, F1-score, Confusion Matrix.  
- **Highlight:** Random Forest and Logistic Regression both achieved ~84% accuracy on the test set .

---

## ⚙️ Installation & Setup
---
```bash
# Clone repo
git clone https://github.com/your-username/heart-disease-ml.git
cd heart-disease-ml

# Create virtual environment
python3 -m venv .venv
source .venv/bin/activate   # Mac/Linux
.venv\Scripts\activate      # Windows

# Install dependencies
pip install -r requirements.txt

# requirements.txt should include:

pandas
numpy
scikit-learn
imbalanced-learn
matplotlib
seaborn
joblib

---

## Summary of Model Performance
--

| Model                  | Accuracy | Precision (Class 0 / 1) | Recall (Class 0 / 1) | Notes |
|-------------------------|----------|--------------------------|-----------------------|-------|
| **Random Forest**       | **84%**  | – / 75%                 | **91%** / 75%         | Best overall, very strong at detecting healthy cases |
| **Logistic Regression** | **83.5%**| >85% both classes        | Slightly lower for Class 1 | Stable, interpretable, balanced |
| **KNN (k=19)**          | 82.4%    | 80% / 85%                | 87% / 77%             | Reliable, good balance |
| **SVM (RBF)**           | 80.2%    | Competitive              | 85% / 75%             | Bias toward majority class (healthy) |
| **Decision Tree**       | 78%      | 68% (Class 1 low)        | 87% / 83%             | Higher false positives |

---


