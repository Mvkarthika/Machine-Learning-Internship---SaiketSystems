📌 Task 1: Data Preparation
🔹 Objective

Prepare the Telco Customer Churn dataset for machine learning by handling missing values, encoding categorical variables, and ensuring data consistency.
🔹 Steps Performed

Dataset Upload

Loaded the dataset (Telco_Customer_Churn_Dataset.csv) into Google Colab using Pandas.

Data Exploration

Checked dataset shape, column data types, and summary statistics.

Identified missing values and categorical variables.

Handling Missing Values

Numerical columns: Replaced missing values with the mean.

Categorical columns: Replaced missing values with the mode.

Encoding Categorical Variables

Binary categorical features (Yes/No): Applied Label Encoding (0/1).

Multi-category features: Applied One-Hot Encoding using pd.get_dummies() (drop_first=True to avoid multicollinearity).

Verification

Confirmed no missing values remained.

Verified all features were numeric and dataset was ML-ready.
🔹 Tools & Libraries

Python

Pandas

NumPy

Scikit-learn

Google Colab
🔹 Skills Practiced

✅ Data preprocessing techniques
✅ Handling missing values
✅ Categorical variable encoding
✅ Preparing data for ML pipeline

🔹 Outcome

The dataset is now clean, consistent, and machine-learning ready, forming the foundation for further tasks like data splitting, feature selection, and model training.
