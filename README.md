To run Breast Cancer DGE dataset on notebook, the following steps are needed:

### 1.	Import Libraries ###

•  Import necessary libraries, including numpy, seaborn, pandas, matplotlib.pyplot, sklearn modules (such as train_test_split, StandardScaler, classification_report, precision_recall_fscore_support, roc_auc_score, etc.),   and imbalanced-learn for SMOTE.

### 2.	Load Data ###
 
  •	Load three CSV datasets (GSE52194.csv, GSE69240.csv, GSE71651.csv) into separate DataFrames (df1, df2, df3).
 
  •	Concatenate these DataFrames into a single DataFrame (df).

### 3.	Data Preprocessing ###

  •	Drop the "ID" column.
  
  •	Transform the "class" column into binary labels (0 for non-tumor, 1 for tumor).
  
  •	Check unique values in the "class" column.

### 4.	Data Exploration ###

  •	Visualize the dataset using PCA for dimensionality reduction.
  
  •	Split the dataset into training and testing sets using SMOTE for oversampling.

### 5.	Model Training: ###

  •	Train various machine learning models (Logistic Regression, K Nearest Neighbors, Linear SVM, RBF SVM, Gaussian Process, Decision Tree, Random Forest, Neural Net, AdaBoost, Naive Bayes, Quadratic Discriminant Analysis).
  
  •	Use a loop to fit each model, print its accuracy, and evaluate its performance.
###  6.	Model Evaluation ###
 
  •	Print classification reports, precision, recall, F1-score, and ROC AUC for each model.
  
  •	Print Confusion Matrix with TP, TN, FP, FN and accuracy

### 7.	Best Performing Models ###
  
  •	Identify and highlight the best-performing models based on accuracy.

### 8.	Comparison Graphs ###
  
  •	Create a heatmap comparing precision, recall, F1 score, accuracy, and ROC AUC for each model.
  
  •	Generate a linear plot representing classification report metrics.

### 9.	Feature Selection ###
  
  •	Apply Univariate Feature Selection (UFS) with PCA to extract top features related to the tumor class genes. (F1_score)

### 10.	Visualizations ###
  
  •	Create linear plot and pairplot of extracted features.
  
  •	Generate a heatmap showing the correlation between top genes.
  
  •	Display a bar plot depicting the average PCA values of top genes.

