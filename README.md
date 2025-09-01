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

📌 Task 2: Data Splitting
🔹 Objective

Split the Telco Customer Churn dataset into training (80%) and testing (20%) sets for fair model training and evaluation, ensuring the split is representative of the target variable distribution.

🔹 Steps Performed

Dataset Upload

Loaded the preprocessed dataset (Telco_Customer_Churn_Dataset.csv) into Google Colab.

Feature/Target Separation

Defined features (X) as all columns except Churn.

Defined target (y) as the Churn column.

Train-Test Split

Used scikit-learn’s train_test_split function.

Parameters:

test_size=0.2 → 20% for testing, 80% for training

random_state=42 → ensures reproducibility

stratify=y → maintains class balance of churn vs. non-churn customers

Basic Checks

Verified training/testing set shapes.

Confirmed target variable distribution is preserved in both splits.

🔹 Tools & Libraries

Python

Pandas

NumPy

Scikit-learn

Google Colab

🔹 Skills Practiced

✅ Data splitting methodologies
✅ Understanding training/testing dataset requirements
✅ Ensuring reproducible and representative splits

🔹 Outcome

The dataset was successfully divided into train (80%) and test (20%) sets, ensuring fair model evaluation and avoiding data leakage in future tasks.

📌 Task 3: Feature Selection & Correlation Analysis
🔹 Objective

Identify the most influential features contributing to customer churn by applying correlation analysis and domain knowledge.

🔹 Steps Performed

Dataset Upload

Loaded the preprocessed dataset (Telco_Customer_Churn_Dataset.csv) into Google Colab.

Feature-Target Correlation

Calculated correlation of all features with the target variable Churn.

Ranked features based on absolute correlation values.

Top Features Selection

Identified Top 10 most influential features affecting churn.

Focused on attributes like tenure, contract type, internet service, monthly charges, etc.

Correlation Heatmap

Created a heatmap visualization of the top 10 features.

Helped in spotting feature relationships and multicollinearity.

Domain Knowledge Validation

Verified feature importance with business understanding.

Example: Short tenure, high monthly charges, and contract type are logically linked to higher churn rates.

🔹 Tools & Libraries

Python

Pandas

NumPy

Seaborn

Matplotlib

Scikit-learn

Google Colab

🔹 Skills Practiced

✅ Feature selection techniques
✅ Correlation analysis
✅ Visualization with heatmaps
✅ Applying domain knowledge to validate attributes

🔹 Outcome

Identified the Top 10 features influencing customer churn with statistical support and business logic.
This step ensures better model interpretability and improves prediction accuracy by focusing on the most relevant attributes.

📌 Task 6: Model Evaluation
🔹 Objective

Evaluate the performance of a Logistic Regression model built on the Telco Customer Churn dataset using multiple classification metrics.

🔹 Steps Performed

Dataset Upload

Loaded the preprocessed dataset (Telco_Customer_Churn_Dataset.csv) into Google Colab.

Train-Test Split

Used the 80/20 split from Task 2 for fair evaluation.

Ensured stratification to maintain class balance.

Model Training

Trained a Logistic Regression model using the selected features from Task 3.

Predictions

Made predictions on the test dataset.

Evaluation Metrics

Calculated:
✔️ Accuracy Score
✔️ Precision
✔️ Recall
✔️ F1-Score

Confusion Matrix Visualization

Plotted a confusion matrix heatmap in shaded pink for intuitive interpretation.

Highlighted true positives, true negatives, false positives, and false negatives.

🔹 Tools & Libraries

Python

Pandas

NumPy

Scikit-learn

Seaborn

Matplotlib

Google Colab

🔹 Skills Practiced

✅ Model training with Logistic Regression
✅ Classification metrics interpretation
✅ Confusion matrix analysis
✅ Visualization of evaluation results

🔹 Outcome

Successfully evaluated a baseline model for customer churn prediction.
Gained insights into model performance beyond accuracy, emphasizing the role of precision, recall, and F1-score for better decision-making in churn prediction.
