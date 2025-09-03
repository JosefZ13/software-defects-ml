\# Machine Learning for Software Defect Prediction – Bachelor Thesis



This repository contains the code, datasets, and analysis for my bachelor thesis:  

\*\*Machine Learning for Software Defect Prediction: A Comparative Study\*\*



---



\## 📂 Repository Structure



software-defects-ml/

├── data/ # NASA PROMISE datasets (JM1, KC1, KC2, PC1, CM1)

├── notebooks/ # Jupyter notebooks (01–10)

│ ├── 01\_data\_preprocessing.ipynb

│ ├── 02\_basic\_models.ipynb

│ ├── 03\_smote\_and\_boosting.ipynb

│ ├── 04\_ann.ipynb

│ ├── 05\_kc1\_experiments.ipynb

│ ├── 06\_curves.ipynb

│ ├── 07\_error\_analysis.ipynb

│ ├── 08\_Hyperparameter\_Tuning.ipynb

│ ├── 09\_NTuning\_vs\_Tuning.ipynb

│ └── 10\_final\_model\_comparison.ipynb

├── report/ # Thesis report (PDF/Word)

├── presentation/ # PowerPoint presentation

├── README.md

├── requirements.txt # Python dependencies

└── .gitignore





---



\## 📊 Pipeline Overview



The project follows a step-by-step machine learning pipeline:



1\. \*\*Data Preprocessing\*\* → cleaning, scaling, stratified train/test splits  

2\. \*\*Basic Models\*\* → Logistic Regression, Random Forest, XGBoost, ANN  

3\. \*\*SMOTE and Boosting\*\* → handling class imbalance  

4\. \*\*Artificial Neural Network\*\* → ANN performance evaluation  

5\. \*\*KC1 Experiments\*\* → dataset-specific experiments  

6\. \*\*Curves\*\* → ROC and Precision-Recall visualization  

7\. \*\*Error Analysis\*\* → FP/FN breakdowns  

8\. \*\*Hyperparameter Tuning\*\* → parameter optimization  

9\. \*\*Normal vs Tuned Models\*\* → comparison of performance  

10\. \*\*Final Model Comparison\*\* → summary across all datasets



---



\## ⚙️ Setup Instructions



\### 1. Install dependencies

```bash

pip install -r requirements.txt



2\. Start Jupyter



jupyter lab



3\. Run the notebooks



Open the notebooks in /notebooks and run the cells in order.

Example (Random Forest with and without SMOTE):



&nbsp;   Shows class distribution



&nbsp;   Applies stratified split



&nbsp;   Runs baseline RF



&nbsp;   Applies SMOTE



&nbsp;   Compares results with confusion matrix, ROC and PR curves



📈 Key Evaluation Metrics



&nbsp;   Accuracy → overall correctness



&nbsp;   Precision → how many predicted defects are truly defects



&nbsp;   Recall (Sensitivity) → how many actual defects were found



&nbsp;   F1-score → balance of precision and recall



&nbsp;   AUC → ability to distinguish classes



💡 Notes for Confusion Matrix (for examiners)



&nbsp;   True Positive (TP): Predicted defect and it was a defect ✅



&nbsp;   False Positive (FP): Predicted defect but it was clean (extra QA effort) ⚠️



&nbsp;   False Negative (FN): Predicted clean but it was a defect (worst case – missed bug) ❌



&nbsp;   True Negative (TN): Predicted clean and it was clean ✅



👉 In defect prediction, recall (catching more defects) is often prioritized to reduce FN.

🙋 Author



Josef Ziada

Bachelor Thesis – University West, 2025

