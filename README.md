### Project Title: Evaluation and Comparison of Classification Models

**Objective:**  
To evaluate and compare different classification models using standard model evaluation metrics with help from the scikit-learn documentation

**Implementation:**

1. **Data Preparation:**
   - Loaded the breast cancer dataset from scikit-learn.
   - Split the data into training (50%), validation (25%), and test (25%) sets using `train_test_split` with stratification.

2. **Model Training and Evaluation:**
   - **Logistic Regression:**
     - Trained a Logistic Regression model with `solver='lbfgs'` and `max_iter=3000`.
     - Evaluated the model using accuracy, recall, precision, AUC, and F1 score.
     - Results:
       - Accuracy: 0.944
       - Recall: 0.966
       - Precision: 0.945
       - AUC: 0.988
       - F1 Score: 0.956

   - **Support Vector Machine (SVM):**
     - Trained an SVM model with `probability=True`.
     - Evaluated the model using the same metrics.
     - Results:
       - Accuracy: 0.894
       - Recall: 0.978
       - Precision: 0.870
       - AUC: 0.967
       - F1 Score: 0.967 (with optimized C value of 100000)

3. **Hyperparameter Tuning:**
   - Optimized the SVM model's hyperparameter `C` to achieve the best F1 score.
   - Tested various values of `C` and found the best value to be 100000.

4. **Model Selection:**
   - Compared the performance of Logistic Regression and SVM.
   - Chose Logistic Regression for its balance of performance, speed, and ease of understanding, despite SVM's higher F1 score.

**Skills Demonstrated:**
- Proficiency in Python and scikit-learn.
- Understanding of classification models and evaluation metrics.
- Experience with data splitting and stratification.
- Knowledge of hyperparameter tuning and model optimization.
- Ability to interpret and compare model performance.

**Tools and Libraries Used:**
- Python
- scikit-learn
- NumPy
