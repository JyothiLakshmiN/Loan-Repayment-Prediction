# Loan Repayment Prediction Using Ensemble Learning Methods

## Objective
This project aims to predict whether a bank should approve a loan for an applicant based on various financial attributes using **Ensemble Learning techniques** such as Decision Trees, Bagging, AdaBoost, Random Forest, and Gradient Boosting.

---

## 📂 Dataset
The dataset used is **`loan_data.csv`**, which includes features such as:
- `credit.policy`
- `purpose`
- `int.rate`
- `installment`
- `log.annual.inc`
- `dti`
- `fico`
- `days.with.cr.line`
- `revol.bal`
- `revol.util`
- `inq.last.6mths`
- `delinq.2yrs`
- `pub.rec`
- `not.fully.paid` *(Target Variable)*

**No missing values** were found in the dataset.  
Categorical columns like `purpose` were encoded using `LabelEncoder`.

---

## Steps Involved
1. **Data Preprocessing**
   - Encoded categorical attributes  
   - Scaled features where necessary  
   - Checked for null values and data types  

2. **Exploratory Data Analysis (EDA)**
   - Visualized relationships between `fico`, `int.rate`, and loan repayment status  
   - Analyzed feature correlations using heatmaps  

3. **Model Training and Evaluation**
   Models applied:
   - Decision Tree Classifier  
   - Bagging with Decision Tree  
   - AdaBoost with Decision Tree  
   - Random Forest Classifier  
   - AdaBoost with Random Forest  
   - Gradient Boosting Classifier  

   Evaluation Metrics:
   - Accuracy  
   - Precision, Recall, F1-score  
   - Confusion Matrix  

---

## Results
| Model | Accuracy |
|--------|-----------|
| Decision Tree | 84.6% |
| Bagging (DT) | 73.1% |
| AdaBoost (DT) | 84.0% |
| **Random Forest** | **85.0%** |
| AdaBoost (RF) | 84.7% |
| Gradient Boosting | 84.4% |

**Best Model:** Random Forest Classifier  
**Accuracy:** 85%  

Observation:  
Most ensemble methods performed similarly, with Random Forest showing the highest accuracy. The dataset exhibited class imbalance, slightly lowering recall for loan defaults.

---

## Technologies Used
- Python  
- NumPy, Pandas  
- Matplotlib, Seaborn  
- Scikit-learn  

---

## Future Improvements
- Apply **SMOTE** or class-weight balancing for imbalanced data.  
- Tune hyperparameters for better performance.  
- Add **ROC-AUC** and **feature importance** visualization.  

---

## Submitted By
**Name:** Jyothi Lakshmi Nagaraj 

---

## 🧾 License
This project is for educational purposes and part of coursework.  
Feel free to use or adapt with proper credit.

