# Online Fraud Detection using Machine Learning


# Project Overview
Online financial fraud is a serious problem faced by banks, payment gateways, and e-commerce platforms.  
This project builds a **machine learning–based fraud detection system** that identifies whether an online transaction is **fraudulent or genuine**.

The key challenge addressed in this project is **highly imbalanced data**, where fraudulent transactions are extremely rare compared to genuine ones.

This repository is designed to act like a **project website**, explaining the problem, approach, and results in a clear and structured way.


# Problem Statement
To detect fraudulent online transactions using historical transaction data while handling the challenge of class imbalance and focusing on meaningful evaluation metrics.


# Objectives
- Detect fraudulent transactions accurately  
- Handle highly imbalanced datasets  
- Improve **recall** for fraud cases  
- Compare baseline and advanced ML models  
- Build a solution suitable for real-world financial systems  


# Dataset Information
- **Source:** Kaggle – Credit Card Fraud Detection Dataset  
- **Total Records:** 284,807  
- **Fraud Transactions:** ~0.17%  
  Target Column: `Class`  
  - `0` → Genuine Transaction  
  - `1` → Fraudulent Transaction  

The dataset is not uploaded to this repository due to GitHub file size limits.  
You can download it directly from Kaggle.



# Technologies & Tools Used
- Python  
- Jupyter Notebook  
- Pandas, NumPy  
- Scikit-learn  
- Imbalanced-learn (SMOTE)  
- Matplotlib & Seaborn  


# Project Workflow
1. Dataset loading and inspection  
2. Exploratory Data Analysis (EDA)  
3. Visualization of fraud vs genuine transactions  
4. Feature scaling (Amount & Time)  
5. Train-test split with stratification  
6. Baseline model using Logistic Regression  
7. Handling class imbalance using **SMOTE**  
8. Final model using **Random Forest Classifier**  
9. Model evaluation using Precision, Recall, and F1-Score  


# Machine Learning Models

# Logistic Regression (Baseline Model)
- Achieved high accuracy
- Performed poorly on fraud recall due to class imbalance
- Demonstrates why accuracy alone is misleading

# Random Forest + SMOTE (Final Model)
- SMOTE balanced the training data
- Random Forest captured complex patterns
- **Significant improvement in fraud recall**
- Better suited for real-world fraud detection



# Results Summary
- Baseline Logistic Regression:
  - Fraud Recall ≈ **0.61**
- Final Random Forest + SMOTE:
  - Fraud recall improved significantly
  - Better detection of rare fraud cases

Key takeaway: 
In fraud detection, **recall is more important than accuracy**, because missing fraud is costly.



# Visual Results
The repository includes visual outputs such as:
- Fraud vs Genuine transaction distribution  
- Confusion matrix of the final model  

These visuals help in understanding model behavior clearly.

---

 # Key Learnings
- Imbalanced datasets require special handling
- Accuracy is not a reliable metric for fraud detection
- SMOTE is effective for balancing rare classes
- Ensemble models perform better for complex patterns
- Model evaluation metrics must align with business goals



# How to Run This Project
1. Clone this repository  
2. Open `Online_Fraud_Detection.ipynb` in Jupyter Notebook  
3. Download the dataset from Kaggle  
4. Place the dataset inside a `dataset/` folder  
5. Run all cells from top to bottom  


  Conclusion
This project demonstrates a practical machine learning approach to online fraud detection.  
By addressing class imbalance and choosing appropriate evaluation metrics, the final model provides a strong foundation for deployment in real-world financial systems.



## 👤 Author
Jasnoor Singh
Bachelor of Engineering in CSE
Machine Learning Project – Online Fraud Detection  
