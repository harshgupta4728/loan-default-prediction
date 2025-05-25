# Loan Default Prediction

## 🏦 Context
A major portion of retail bank profits comes from home loans borrowed by regular or high-income customers. However, defaults (non-performing assets) can significantly affect bank profitability. The traditional manual loan approval process is time-consuming and subject to human error and bias. This project aims to automate and enhance the decision-making process using machine learning models that are fair, interpretable, and efficient.

---

## 📌 Problem Statement
A bank’s consumer credit department wants to develop a reliable credit scoring model to predict whether a loan applicant is likely to default. The model must:
- Comply with Equal Credit Opportunity Act guidelines.
- Be interpretable to explain decisions (especially rejections).
- Be based on the historical performance of previously approved loans.

---

## 🎯 Objective
- Build a binary classification model that predicts whether a client will default (BAD = 1) or repay (BAD = 0).
- Identify key features influencing default likelihood.
- Recommend criteria to aid banks in making data-driven and fair lending decisions.

---

## 📂 Dataset Information
The dataset is based on the **Home Equity Line of Credit (HMEQ)** data, with the following attributes:

| Feature | Description |
|---------|-------------|
| BAD | Target variable (1 = defaulted, 0 = repaid) |
| LOAN | Approved loan amount |
| MORTDUE | Amount due on existing mortgage |
| VALUE | Current value of the property |
| REASON | Reason for the loan (HomeImp, DebtCon) |
| JOB | Type of employment |
| YOJ | Years at current job |
| DEROG | Number of major derogatory reports |
| DELINQ | Number of delinquent credit lines |
| CLAGE | Age of oldest credit line |
| NINQ | Number of recent credit inquiries |
| CLNO | Number of existing credit lines |
| DEBTINC | Debt-to-income ratio |

---

## 🧠 Models Used
- Logistic Regression
- Decision Tree (Baseline & Tuned)
- Random Forest

### ✅ Final Model: Tuned Decision Tree
| Metric | Score |
|--------|-------|
| Accuracy | 0.86 |
| Recall | 0.74 |
| Precision | 0.62 |

> This model was selected due to its **high interpretability** and **strong recall**, making it effective at minimizing the number of defaulters misclassified as safe.

---

## 🛠️ Tech Stack
- Python
- pandas, NumPy
- matplotlib, seaborn
- scikit-learn

---

## 📌 Key Steps
1. **Data Cleaning & Preprocessing**
   - Handling missing values
   - Outlier detection
   - Encoding categorical variables
   - Feature scaling

2. **Exploratory Data Analysis (EDA)**
   - Univariate & bivariate analysis
   - Correlation heatmaps
   - Boxplots & histograms

3. **Model Building**
   - Baseline and tuned models
   - Evaluation using cross-validation

4. **Model Evaluation**
   - Accuracy, Precision, Recall, F1-Score
   - Confusion matrix analysis

---

## 📈 Outcome
- Built an effective credit risk model with a strong focus on reducing false negatives (defaulters predicted as safe).
- Identified critical features like **Debt-to-Income Ratio, Job Type, Delinquency Count**, and **Credit Line Age** that influence loan defaults.

---

## 📝 Future Work
- Integrate SHAP/ELI5 for advanced model interpretability.
- Deploy model using Flask/Streamlit for real-time predictions.
- Explore ensemble models like XGBoost or LightGBM.

---

## 🙋‍♂️ Author
Harsh Gupta  
Email: [your-email@example.com]  
LinkedIn: [your-linkedin-profile]  

---

