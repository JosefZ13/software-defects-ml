### Machine Learning For Software defect Prediction



This repository contains the code, datasets, and analysis for my bachelor thesis:



Machine Learning For Software Defect Prediction: A Comparative Study



##### Repository Structure 



software-defects-ml/

├── data/ 					# NASA PROMISE datasets (JM1, KC1, KC2, PC1, CM1)

├── notebooks/ 			# Jupyter notebooks (01–10)

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

├── README.md

├── requirements.txt 		# Python dependencies

└── .gitignore



##### Notebooks Overview

| Notebook 				| Description 													|

|----------				|-------------													|

| 01\_data\_preprocessing.ipynb 		| Loads datasets (JM1, KC1, KC2, PC1, CM1), cleans and scales features, applies stratified train/test split. 	|

| 02\_basic\_models.ipynb 		| Trains baseline models (Logistic Regression, Random Forest, XGBoost, ANN) without balancing. 			|

| 03\_smote\_and\_boosting.ipynb		| Applies SMOTE to balance classes, retrains models, compares performance before/after. 			|		

| 04\_ann.ipynb 				| Focus on Artificial Neural Networks (MLP), performance evaluation, sensitivity to class imbalance. 		|

| 05\_kc1\_experiments.ipynb		| Dataset-specific experiments on KC1 with visualizations and comparisons. 					|

| 06\_curves.ipynb			| Generates ROC and Precision–Recall curves for all models. 							|

| 07\_error\_analysis.ipynb		| Analyzes false positives/negatives, provides error breakdown. 						|

| 08\_Hyperparameter\_Tuning.ipynb 	| Performs hyperparameter tuning (e.g. GridSearchCV) to optimize models. 					|

| 09\_NTuning\_vs\_Tuning.ipynb 		| Compares models with default parameters vs tuned models. 							|

| 10\_final\_model\_comparison.ipynb 	| Summarizes results across datasets and models, provides final comparison and insights. 			|



###### Setup Instructions:



1\. Install dependencies

&nbsp;	pip install -r requirements.txt

2\. Start Jupyter

&nbsp;	jupyter lab

3\. Run the notebooks

&nbsp;	Open the notebooks in "/notebooks" and run the cells in order.



##### Key Evaluation Metrics



Accuracy -> overall correctness

Precision -> how many predicted defects are truly defects

Recall (Sensitivity) -> how many actual defects were found

F1-score -> balance of precision and recall

AUC -> ability to distinguish classes



Notes for Confusion Matrix



True Positive (TP): Predicted defect and it was a defect

False Positive (FP): Predicted defect was clean 

False Negative (FN): Predicted clean but it was a defect

True Negative (TN): Predicted clean and it was clean



Author

Josef Ziada 

Bachelor Thesis - University West ,  2025

