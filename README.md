
Credit Card Fraud Detection using Machine Learning

This project aims to build a robust machine learning model to detect fraudulent credit card transactions with high accuracy. The model is trained on a real-world dataset from Kaggle and addresses the challenge of class imbalance using SMOTE.

Objective
Detect and classify credit card transactions as fraudulent or non-fraudulent using machine learning algorithms to reduce financial risk and loss.

Dataset Overview
- **Source**: [Kaggle - Credit Card Fraud Detection(https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)
- **Rows**: 284,807
- **Features**: 31 total
  - `Time`, `Amount`, `V1` to `V28` (anonymized), `Class` (target variable)
- **Class Distribution**: Highly imbalanced (~0.172% fraudulent cases)

Data Preprocessing
- Checked for missing values: None found
- Removed 1,081 duplicate records
- Data split: 70% training / 30% testing
- Applied SMOTE to balance the target classes

Exploratory Data Analysis (EDA)
- Visualized fraud vs. non-fraud distribution
- Analyzed transaction `Time` and `Amount`
- Generated correlation heatmap to inspect feature relationships

Models Trained
- Logistic Regression
- K-Nearest Neighbors (KNN)
- Decision Tree
- Random Forest
- AdaBoost
- XGBoost

Best Model: K-Nearest Neighbors (KNN)
- **Accuracy**: 99.4%
- **F1-Score**: 81%
- **Why KNN?**
  - Robust to overfitting
  - Balanced performance for both classes
  - High precision and recall for the minority class

Conclusion
- Developed a reliable ML model for fraud detection
- Successfully handled class imbalance with SMOTE
- Achieved high performance with KNN classifier

How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/credit-card-fraud-detection.git
   cd credit-card-fraud-detection
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the model script:
   ```bash
   python fraud_detection.py
   ```

License
This project is licensed under the MIT License.

---
🔗 Developed by Prajkta Chodankar | April 2025

