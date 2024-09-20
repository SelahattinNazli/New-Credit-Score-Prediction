
# Home Equity Loan Default Prediction

## Project Overview

The objective of this project is to build a predictive model to automate the decision-making process for approving **home equity lines of credit (HELOCs)**. The model aims to identify whether an applicant is likely to default on a home equity loan. This project is conducted in line with the guidelines of the **Equal Credit Opportunity Act (ECOA)** to ensure that the credit scoring model is both **empirically derived** and **statistically sound**. Additionally, the model must be sufficiently interpretable to provide justifications for any adverse actions (loan rejections) as required by law.

The dataset used in this project is known as the **HMEQ (Home Equity)** dataset, which contains historical data on applicants for home equity loans and their outcomes. The key goal is to predict whether an applicant will default or have serious delinquencies in their loan payments.

## Dataset Overview

The dataset consists of **5,960** recent home equity loan applications. The target variable is **`BAD`**, which is a binary classification variable indicating whether an applicant defaulted or experienced severe delinquency. Approximately **20%** of the applicants in the dataset defaulted or had significant delinquencies. 

### Key Variables in the Dataset:
- **`BAD`**: Binary target variable where `1` indicates default or serious delinquency, and `0` indicates no default.
- **`LOAN`**: The loan amount requested by the applicant.
- **`MORTDUE`**: Amount due on the existing mortgage.
- **`VALUE`**: Appraised value of the property.
- **`REASON`**: The reason for the loan request (either for home improvement or debt consolidation).
- **`JOB`**: Applicant's job category.
- **`YOJ`**: Years the applicant has been in their current job.
- **`DEROG`**: Number of major derogatory credit reports.
- **`DELINQ`**: Number of delinquent credit lines.
- **`CLAGE`**: Age of the oldest credit line in months.
- **`NINQ`**: Number of recent credit inquiries.
- **`CLNO`**: Number of credit lines the applicant has.
- **`DEBTINC`**: Debt-to-income ratio of the applicant.

## Project Goals

1. **Build a Predictive Model**: The goal is to create a model that can predict the likelihood of default for loan applicants based on their financial and demographic information.
   
2. **Interpretability**: The model needs to be interpretable, as any loan rejection must be justified based on specific applicant data. This is in compliance with the **Equal Credit Opportunity Act (ECOA)**.

3. **Handle Class Imbalance**: Since only 20% of applicants defaulted, the project will handle the class imbalance problem by using techniques like **SMOTE** (Synthetic Minority Over-sampling Technique) and model evaluation methods like **ROC-AUC**.

4. **Evaluate Model Performance**: Evaluate the model using metrics such as **accuracy**, **precision**, **recall**, **F1-score**, and **ROC-AUC**. Models like **Random Forest**, **Logistic Regression**, **Support Vector Machine (SVM)**, and **K-Nearest Neighbors (KNN)** will be used and compared.

## Steps in the Project

1. **Exploratory Data Analysis (EDA)**: Analyze the dataset to understand missing values, distributions, and correlations between features.
2. **Data Preprocessing**:
   - Handle missing values.
   - Encode categorical variables (`REASON` and `JOB`).
   - Scale numerical features as required.
3. **Modeling**:
   - Train multiple machine learning models to predict loan default.
   - Apply **SMOTE** to address the class imbalance problem.
4. **Model Evaluation**:
   - Compare models using metrics such as **accuracy**, **precision**, **recall**, **F1-score**, and **ROC-AUC**.
   - Plot **ROC curves** for each model.
5. **Feature Importance**:
   - Use models like **Random Forest** to identify the most important features influencing the prediction.

## Technologies Used

- **Python**: Programming language used for data processing and modeling.
- **Pandas**: For data manipulation and cleaning.
- **Scikit-learn**: For machine learning models, SMOTE, and evaluation metrics.
- **Matplotlib/Seaborn**: For data visualization.
- **Joblib**: For saving trained machine learning models.

## Conclusion

This project aims to build a robust, interpretable model to assist the bank in automating home equity loan approval decisions. The model helps in predicting the probability of default for loan applicants, ensuring that the credit decision-making process is both efficient and compliant with regulations.

By providing an empirical and statistically sound credit scoring model, the bank can ensure fair and transparent decisions while minimizing the risk of loan defaults.

---


