# 🩺 Diabetes Prediction: Ensemble Learning Benchmark

## 📌 Business Overview
Diabetes is a chronic condition where early detection significantly improves patient outcomes. This project compares **10 different Machine Learning algorithms** to build a robust diagnostic tool that can predict diabetes risk using standard clinical metrics (Glucose, BMI, Age), enabling healthcare providers to prioritize at-risk patients.

## 📊 Technical Approach
This project focuses on **Model Selection** and **Ensemble Techniques**.

* **Data Cleaning:** Detected and imputed missing values hidden as "0" (e.g., a Glucose level of 0 is impossible) using median replacement.
* **Algorithms Tested:**
    1.  **Ensemble Methods:** Random Forest, Bagging Classifier, Voting Classifier, XGBoost.
    2.  **Traditional Models:** Logistic Regression, SVM, KNN, Naive Bayes.
    3.  **Neural Networks:** Basic MLP Classifier.
* **Evaluation Metric:** Focus on **AUC-ROC** (Area Under Curve) to measure the model's ability to distinguish between classes, rather than just raw accuracy.

## 📈 Key Findings
1.  **Ensemble Superiority:** Tree-based ensemble methods (Bagging, Random Forest) consistently outperformed single models, achieving an **AUC of 0.82**.
2.  **Feature Importance:** `Glucose` concentration was the single most predictive feature, followed by `BMI` and `Age`.
3.  **Model Stability:** The **Voting Classifier** provided a balanced trade-off between sensitivity (catching cases) and specificity (reducing false alarms).

## 🛠 Tools Used
* **Python:** Scikit-Learn, XGBoost, Pandas
* **Visualization:** Seaborn Heatmaps (Model Comparison Matrix)
* **Techniques:** Cross-Validation, Hyperparameter Tuning, Voting Ensembles

## 🚀 How to Run
1.  Clone the repository.
2.  Install dependencies: `pip install -r requirements.txt`
3.  Run the notebook `ML Final Project Code File.ipynb`.
