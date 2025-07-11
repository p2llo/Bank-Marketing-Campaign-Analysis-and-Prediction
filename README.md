# Bank-Marketing-Campaign-Analysis-and-Prediction

#Project Overview : 
This project analyzes the UCI Bank Marketing dataset to understand customer behavior and predict whether a client will subscribe to a term deposit. The analysis includes data cleaning, exploratory data analysis (EDA), preprocessing, and training multiple classification models to evaluate their performance in predicting subscription outcomes.
#Dataset
The dataset (bankmarketing.csv) is sourced from the UCI Machine Learning Repository and contains information about a bank's marketing campaigns. Key features include:

Demographic: Age, job, marital status, education
Financial: Balance, housing loan, personal loan
Campaign: Contact type, day, month, duration, campaign contacts
Target Variable: y (binary: 'yes'/'no' for term deposit subscription)

#Project Structure

bankmarketing.csv: Input dataset
data_cleaning.py: Handles missing values and basic data cleaning
eda.py: Performs exploratory data analysis with visualizations
preprocessing.py: Encodes categorical variables and normalizes numerical features
data_splitting.py: Splits data into training and testing sets
model_training.py: Trains Logistic Regression, Decision Tree, and Random Forest models
model_evaluation.py: Evaluates model performance using accuracy, precision, recall, and F1-score



#Usage

Open a Jupyter notebook.
Run the code cells in the following order:
Load and inspect the dataset (df = pd.read_csv('bankmarketing.csv'))
Run data_cleaning.py to handle missing values
Run eda.py to explore data patterns
Run preprocessing.py to encode and normalize features
Run data_splitting.py to split data
Run model_training.py to train models
Run model_evaluation.py to evaluate model performance


Review outputs (visualizations, metrics) in the notebook.

#Results

EDA: Visualizations reveal relationships between features (e.g., age, job, balance) and the target variable.
Preprocessing: Categorical features are one-hot encoded, and numerical features are normalized.
Model Performance: Logistic Regression, Decision Tree, and Random Forest models are evaluated using accuracy, precision, recall, and F1-score.

#Notes

The target variable is assumed to be y (binary: 'yes'/'no'). Adjust column names in the code if your dataset uses a different name (e.g., deposit).
If errors occur (e.g., missing columns like balance), check column names using df.columns.tolist() and update the code accordingly.
For imbalanced datasets, consider techniques like SMOTE or adjusting class weights in models.

