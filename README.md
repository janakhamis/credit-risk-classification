# Credit Risk Classification

## An overview of the analysis

The purpose of this analysis is to develop a machine learning model that can determine if a loan is high-risk (1) or healthy (0). The dataset includes financial information such as loan amount, interest rates, borrower income, and other relevant features. The objective is to develop a model that can properly categorize loans into these two groups.

**Target Variable (loan_status)**
The target variable in this classification problem is loan_status, which indicates whether a loan is:
  - 0 (Healthy Loan): The borrower is likely to repay the loan.
  - 1 (High-Risk Loan): The borrower is at risk of defaulting.

**Machine Learning Process**
The stages of the machine learning process include:
  - Loading and preprocessing the dataset.
  - Splitting the data into training and testing sets to evaluate model performance.
  - Training a logistic regression model to classify loans as healthy or high-risk.
  - Evaluating model performance using classification metrics such as accuracy, precision, and recall.

## Results
**Machine Learning Model: Logistic Regression:**
 1. **Accuracy: 99%**
 
    The overall accuracy of the model is very high, meaning that 99% of the loan classifications were correct.

 2. **Precision:**
    * Class 0 (Healthy Loan): 1.00
      * Every loan predicted as "healthy" was indeed healthy. This means there were no false positives for class 0.
    * Class 1 (High-Risk Loan): 0.87
      *  Out of all loans predicted as "high-risk," 87% were actually high-risk. A lower precision for class 1 indicates some healthy loans were incorrectly classified as high-risk.
 3. **Recall:**
    * Class 0 (Healthy Loan): 1.00
      * The model successfully identified all healthy loans without missing any, meaning there were no false negatives for class 0.
    * Class 1 (High-Risk Loan): 0.95
      * The model correctly identified 95% of the actual high-risk loans, though it missed 5% (false negatives).

## Summary
The logistic regression model works remarkably well, with a 99% accuracy rate. However, there is a minor difference in accuracy and recall for class 1 (high-risk loans). While the model accurately detects 95% of high-risk loans (high recall), its accuracy is significantly lower (87%), suggesting that some healthy loans may be misclassified as high-risk.

## Recommendation
Given the high accuracy and recall for high-risk loans, this model is suitable if minimizing the risk of failing to identify high-risk loans is the priority. However, if misclassifying healthy loans as high-risk has serious business consequences, alternative models or additional feature engineering may be necessary.

## How to Run it 
1. Clone the repository:
    1. Open your terminal (Git Bash, Command Prompt, or any Git client).
    2. Use the cd command to navigate to the directory where you want to clone the repository.
    3. Run the following command to clone the repository: git clone link_provided
2. Ensure Pandas, Numpy, Pathlib, and Scikit-learn is installed on your machine.
   - Install Pandas using pip if it's not already installed (pip install pandas).
   - Install Numpy using pip if it's not already installed (pip install numpy).
   - Install Pathlib using pip if it's not already installed (pip install pathlib).
   - Install Scikit-learn using pip if it's not already installed (pip install scikit-learn).
3. Open the cloned file in the Visual Studio Code:
   1. Go to file > Open Folder and navigate to the folder where you cloned the repository.
   2. Select the folder to open in VS code.
4. Run the Jupyter Notebook:
     1. Open the notebook file (credit_risk_classification.ipynb) in VS code or Jupyter.
     2. Run the cells to perform the Analysis.