# Logistic-Classification-Model

Greetings,

Welcome to the Logistic-Classification-Model repository! This project contains Python code utilizing Scikit-learn in order to generate a binary classification model from a loan dataset that is capable of determining whether or not a particular loan's attributes/feature data classify it as "Healthy" or "High Risk".

**Repository Structure:**

- 'Credit_Risk' directory:
  - 'Resources' directory: Contains initial CSV file of lending dataset ("lending_data.csv")
  - "credit_risk_classification.ipynb": Code for model generation

**Overview of the Analysis:**

- The dataset contained attribute information for more than 77 thousand individual loans such as loan size, interest rate, borrower income, debt to income ratio, total number of borrower accounts, total number of derogatory marks, total amount of debt and finally our primary outcome/dependent variable loan status, which was represented via a binary value with (0) indicating a "Healthy" loan and (1) indicating a "High Risk" loan.
- In order to instantiate this supervised machine learning model, a traditional workflow was utilized as follows:
  
   - a.) Load and visualize data
  
   - b.) Define feature (input/X) set and label (outcome/y) set

   - c.) Split the data into training and testing datasets

   - d.) Create a Logistic Regression Model and fit it with training (X_train & y_train) data

   - e.) Generate model predictions via the testing (X_test) data

   - f.) Evaluate the model's performance with both a confusion matrix and classification report

**Results:**

- Logistic Regression Machine Learning Model:
  - "Healthy Loan (0)" = Precision: 1.00, Recall: 0.99, F1-Score: 1.00, Support: 18,765
  - "Unhealthy/High Default Risk Loan (1)" = Precision: 0.85, Recall: 0.91, F1-Score: 0.88, Support: 619
  - Overall Accuracy = F1-Score: 0.99, Support: 19,384
  - Macro Avg = Precision: 0.92, Recall: 0.95, F1-Score: 0.94, Support: 19,384
  - Weighted Avg = Precision: 0.99 , Recall: 0.99, F1-Score: 0.99, Support: 19,384

**Summary:**

As evidenced by the confusion matrix and more explicitly by the classification report, our logistic regression model performs very adequately overall with an accuracy score of 99%. Specifically in terms of predicting "Healthy Loans (0)", the model is near perfect with a precision score of 100% and a recall score of 99% - this is becuase our model posesses a significanlty greater number of instances representing a healthy loan. Comparatively, while our model still performs adequately in correctly predicting "Unhealthy/High Default Risk Loans (1)", the limited number of instances representing this classification results in a slightly lower precision score of 85% and recall score of 91%.
