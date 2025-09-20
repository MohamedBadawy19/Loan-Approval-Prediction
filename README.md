# 🏦 Loan Approval Prediction

This project predicts *loan approval status* (Approved/Rejected) based on applicant financial and demographic details using *machine learning classification models*.

---

## 📂 Dataset

The dataset used is *loan_approval_dataset.csv* with *4269 records* and the following features:

- *no_of_dependents* → Number of dependents  
- *education* → Graduate / Not Graduate  
- *self_employed* → Yes / No  
- *income_annum* → Annual income of applicant  
- *loan_amount* → Requested loan amount  
- *loan_term* → Loan repayment term (in years)  
- *cibil_score* → Applicant’s credit score  
- *all_assets_values* → Combined value of residential, commercial, luxury, and bank assets  
- *loan_status* → Target (Approved/Rejected)  

✔ No missing values  
✔ No duplicates  

---

## 🛠 Tools & Libraries

The project uses *Python 3* with the following libraries:

- *pandas* → Data preprocessing  
- *numpy* → Numerical operations  
- *matplotlib / seaborn* → Data visualization  
- *scikit-learn* → Model training & evaluation  

---

## 🔎 Project Workflow

1. *Data Preprocessing*
   - Dropped unnecessary columns (loan_id, individual asset columns).
   - Created a new feature: all_assets_values.
   - Encoded categorical variables (education, self_employed, loan_status).
   - Standardized numerical features with *StandardScaler*.

2. *Exploratory Data Analysis (EDA)*
   - Distribution plots for numerical features.
   - Correlation analysis between income, loan amount, CIBIL score, and loan approval.

3. *Model Training*
   - *Logistic Regression*
   - *Decision Tree Classifier*

4. *Evaluation*
   - Classification report (Precision, Recall, F1-score).
   - Confusion matrix visualization.
   - Accuracy comparison.

---

## 📊 Results & Accuracy

- *Logistic Regression*
  - Accuracy: *~88%*
  - Performed well in classifying both approved and rejected loans.
  
- *Decision Tree Classifier*
  - Accuracy: *~96%*
  - Outperformed Logistic Regression by capturing complex relationships in the dataset.
  
✅ *Best Model: Decision Tree Classifier (96% Accuracy)*

---

## ▶ How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/loan-approval-prediction.git
   cd loan-approval-prediction

2. Install dependencies:

pip install -r requirements.txt


3. Run the Jupyter Notebook:

jupyter notebook loan-approval-prediction.ipynb




---

📌 Future Work

Try Random Forest and XGBoost for potentially higher accuracy.

Perform hyperparameter tuning with GridSearchCV.

Deploy the model using Flask/Streamlit for real-world applications.

