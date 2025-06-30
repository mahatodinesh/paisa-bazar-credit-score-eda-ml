#  Paisa Bazar Credit Score Classification – EDA & Machine Learning

This project analyzes and models a credit score classification problem using a real-world dataset from Paisa Bazar. We perform comprehensive Exploratory Data Analysis (EDA), feature engineering, and implement multiple machine learning models to classify credit scores into Good, Standard, and Poor categories.

---

##  Problem Statement

Financial institutions need to evaluate the creditworthiness of applicants. By predicting the credit score category of a user, lenders can reduce default risk, tailor interest rates, and approve loans more efficiently.  
The goal is to **build a classification model** that predicts whether a user's credit score is `Good`, `Standard`, or `Poor` based on features such as income, EMI, payment history, and more.

---

##  Dataset Overview

The dataset includes user-level financial information:

-  **Numerical Columns**: Age, Annual Income, Monthly EMI, Outstanding Debt, Credit Utilization Ratio, etc.  
-  **Categorical Columns**: Occupation, Credit Mix, Payment Behavior, Credit Score (Target)  
-  **Text Columns**: Loan Types, Payment of Minimum Amount

---

##  Project Workflow

1. **Data Loading & Preprocessing**
   - Handle missing values
   - Drop duplicates
   - Type conversions

2. **Exploratory Data Analysis (EDA)**
   - 15+ interactive charts (boxplots, countplots, heatmaps)
   - Correlation insights
   - Credit score distribution

3. **Feature Engineering**
   - Imputation (mode, mean)
   - Label Encoding & OneHot Encoding
   - Outlier removal
   - Text cleaning (optional for NLP columns)

4. **Model Building**
   - Train/test split
   - ML Models used:
     - Logistic Regression
     - Random Forest Classifier
     - XGBoost Classifier
   - Evaluation metrics:
     - Accuracy
     - Precision / Recall / F1
     - Confusion Matrix

5. **Model Tuning & Cross Validation**
   - GridSearchCV for optimal hyperparameters
   - Comparison of models before & after tuning

6. **Visualization for Business Insights**
   - EMI vs Credit Score
   - Payment Behavior vs Score
   - Debt vs Balance insights

---

##  Key Insights from EDA

- Customers with **higher delayed payments** and **credit utilization** tend to have **Poor scores**.
- Occupations like **Scientist** or **Teacher** are mostly linked with **Good credit scores**.
- Those who pay only the **minimum due** are more likely to have a **Standard or Poor score**.
- Younger users tend to fall into lower score categories.

---

## Technologies Used

- Python 
- Pandas, NumPy for data handling
- Matplotlib, Seaborn for EDA
- Scikit-learn for ML modeling
- XGBoost for advanced modeling
- Streamlit/CapCut (optional) for video visualization

---

## Project Structure

```bash
paisa-bazar-credit-score/
│
├── dataset.csv                      # Cleaned Dataset
├── EDA_visualizations.ipynb         # All 15 charts + EDA code
├── model_training.ipynb             # ML model building & tuning
├── presentation.pptx                # PPT for project explanation
├── video_script.txt                 # Narration for 7-min video
├── README.md                        # This file
