# Credit-Card-Fraud-Detection
# Credit Card Fraud Detection

This repository contains an implementation of **Credit Card Fraud Detection** using machine learning techniques. The project involves dataset preprocessing, model training, evaluation, and performance comparison using multiple classification models.

## **Project Structure**
```
Credit-Card-Fraud-Detection/
│-- notebooks/
│   ├── credit_fraud_updated.ipynb
│-- dataset/
│   ├── creditcard.csv
│-- reports/
│   ├── Credit_Card_Fraud_Detection_Report.docx
│-- presentations/
│   ├── DAMT_Project_Review_Group_10.pptx
│-- .gitignore
│-- README.md
```

## **Dataset Information**
The dataset used in this project is sourced from **Worldline & Université Libre de Bruxelles (ULB)**. It contains **284,807 transactions** recorded over **two days**, where **492 transactions** are fraudulent (~0.172%). The dataset is highly imbalanced and consists of:
- **28 PCA-transformed features** to ensure privacy
- **Two non-PCA features:** `Time` and `Amount`
- **Target Variable (`Class`)**:
  - `1` → Fraudulent transaction
  - `0` → Non-fraudulent transaction

## **Machine Learning Models Implemented**
The project implements and compares multiple machine learning algorithms:
1. **Logistic Regression**
2. **Random Forest Classifier**
3. **Support Vector Machine (SVM)**

### **Performance Comparison**
| Model               | Accuracy | Training Time |
|--------------------|----------|--------------|
| Random Forest      | 95.7%    | 0.77 sec     |
| Logistic Regression | 95.0%    | 0.33 sec     |
| SVM                | 86.3%    | 0.33 sec     |

- **Best Model:** *Random Forest* achieved the highest accuracy and robustness in detecting fraudulent transactions.
- **Evaluation Metrics:** Precision, Recall, F1-score, and the Area Under Precision-Recall Curve (AUPRC) were used due to dataset imbalance.

## **Installation**
1. Clone this repository:
   ```sh
   git clone https://github.com/YOUR_GITHUB_USERNAME/Credit-Card-Fraud-Detection.git
   ```
2. Navigate to the directory:
   ```sh
   cd Credit-Card-Fraud-Detection
   ```
3. Install required dependencies:
   ```sh
   pip install numpy pandas scikit-learn matplotlib seaborn
   ```

## **Usage**
- Open and run the Jupyter Notebook:
  ```sh
  jupyter notebook notebooks/credit_fraud_updated.ipynb
  ```
- Ensure `creditcard.csv` is placed inside the `dataset/` folder before running the notebook.

## **Conclusion**
- The **Random Forest model** provided the best balance of accuracy, recall, and precision, making it the best-suited model for fraud detection.
- The project highlights the importance of handling **imbalanced datasets** and optimizing machine learning models for real-world fraud detection systems.

## **License**
This project is open-source and available for educational use.
