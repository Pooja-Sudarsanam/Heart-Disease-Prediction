## 🫀A Data-Driven Approach to Cardiovascular Disease Prediction
Goal: Build and compare classic ML models to predict heart disease using the Cleveland/UCI dataset.
Models. KNN, Logistic Regression, SVM (RBF), Decision Tree, Random Forest.
Highlights. 70/30 train–test split, z-score scaling, class rebalancing via oversampling, confusion-matrix based evaluation (Accuracy, Precision, Recall, F1).

**📊 Summary of Model Performance**
	•	Random Forest was the top performer (84% accuracy), excelling at detecting healthy individuals (Class 0 recall = 91%) while maintaining balanced metrics for diseased cases (Class 1 precision/recall = 75%).
	•	Logistic Regression closely followed (83.5% accuracy), showing stable precision and recall above 85% overall, though it had a slight drop in recall for Class 1, leading to some missed disease cases.
	•	K-Nearest Neighbors achieved 82.4% accuracy, with well-balanced metrics (precision: 80%/85%, recall: 87%/77%), confirming its reliability in binary classification.
	•	Support Vector Machine (RBF) reached 80.2% accuracy, performing strongly on healthy cases (Class 0 recall = 85%) but lower on disease cases (Class 1 recall = 75%), suggesting bias toward the majority class.
	•	Decision Tree had the lowest accuracy (78%), with decent recall for Class 1 (83%) but poor precision (68%), indicating higher false positives.

**👉 Random Forest and Logistic Regression emerged as the most effective models, balancing interpretability, predictive strength, and recall.**

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

## 🗂️ Project Structure
---

## ⚙️ Installation & Setup

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

requirements.txt should include:

pandas
numpy
scikit-learn
imbalanced-learn
matplotlib
seaborn
joblib


