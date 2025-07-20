# Breast Cancer Detection (using Logistic Regression)
A concise, interpretable machine learning project that trains a logistic regression model to classify breast tumors as benign or malignant using the popular UCI Breast Cancer Wisconsin (Diagnostic) dataset from Kaggle.

##  Dataset

- **Source:** [Kaggle – UCI Breast Cancer Wisconsin Data](https://www.kaggle.com/datasets/uciml/breast-cancer-wisconsin-data)
- **Samples:** 569 instances — 357 benign and 212 malignant  
- **Features:** 30 real-valued measurements (mean, standard error, and “worst” of 10 nucleus attributes) :contentReference[oaicite:1]{index=1}

##  Project Highlights
Data Cleaning:
Removed unnecessary columns such as id and handled any missing or inconsistent data to ensure a clean dataset for model training.

Label Encoding:
Converted the categorical diagnosis column into binary numeric format: Malignant as 1 and Benign as 0 for compatibility with scikit-learn models.

Feature Normalization:
Applied feature scaling using standardization (z-score normalization) to ensure all features contribute equally to the model's performance and improve convergence during training.

Model Training:
Built and trained a logistic regression model using the processed dataset. The model was chosen for its simplicity, interpretability, and efficiency in binary classification problems.

Model Evaluation:
Assessed the model using various performance metrics, including accuracy, precision, recall, F1-score, and ROC AUC. Visualizations such as the confusion matrix and ROC curve were used to interpret results.

Reproducibility:
The entire workflow is encapsulated in a single Jupyter notebook, making it easy to follow and reproduce. Code is modular and well-documented for clarity.

##  Evaluation Metrics
The logistic regression model performs very well on the test set:

Accuracy: 0.98 (98%)

Classification Report:
Class        |  Precision  |   Recall    | F1Score   |Support|
-------------|-------------|-------------|-----------|-------|
Benign (0)   |	0.99	   |   0.98	     |0.99	     |108    |
Malignant (1)|	0.97	   |   0.98	     |0.98	     |63     |
Accuracy	 |		       |             |0.98	     |171    |
Macro Avg	 |  0.98	   |   0.98	     |0.98	     |171    |
Weighted Avg |	0.98	   |   0.98	     |0.98	     |171    |

 Interpretation:
Precision: High precision (0.97–0.99) indicates the model rarely misclassifies benign or malignant tumors.

Recall: Both classes have a recall of ~0.98, showing that the model correctly identifies nearly all positive and negative cases.

F1-score: Balanced F1-scores (~0.98–0.99) confirm strong and consistent performance across both classes.

## Tech Stack
1. Python
2. Pandas, NumPy, Matplotlib, Seaborn
3. Scikit-learn (for preprocessing, model training & evaluation)
4. Jupyter Notebook

Feel free to explore, fork or contribute. Feedback and improvements are always welcome!