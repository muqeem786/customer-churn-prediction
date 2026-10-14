# Customer Churn Prediction Using Machine Learning

## Project Overview
Customer churn prediction is a machine learning project that aims to identify customers who are likely to stop using a company's services. By identifying potential churners, businesses can develop strategies to improve customer retention and reduce customer loss.

This project uses customer data to explore churn patterns and build classification models that predict whether a customer is likely to leave.

## Objectives
- Understand customer churn patterns through Exploratory Data Analysis (EDA).
- Clean and preprocess the dataset for machine learning.
- Handle class imbalance using SMOTE.
- Train and compare multiple classification algorithms.
- Evaluate model performance using appropriate classification metrics.
- Save and load the trained model for future predictions.

## Dataset
The project uses a customer churn dataset containing customer demographics, service subscriptions, account information, billing details, and churn status.

- **Total records:** 7,043 customers
- **Target variable:** Churn
- **Features:** Customer-related demographic, service, and billing information

## Technologies Used
- **Python** — model development and data analysis
- **Pandas & NumPy** — data manipulation
- **Matplotlib & Seaborn** — data visualization
- **Scikit-learn** — preprocessing, model training, and evaluation
- **Imbalanced-learn** — handling class imbalance with SMOTE
- **XGBoost** — gradient boosting classification
- **Jupyter Notebook** — development environment

## Project Workflow

### 1. Data Cleaning and Preprocessing
- Inspected the dataset and checked for missing values.
- Removed the customer ID column, which does not provide useful predictive information.
- Encoded categorical variables into numerical values.
- Separated the input features and target variable.
- Split the data into training and testing sets.

### 2. Exploratory Data Analysis (EDA)
- Analyzed numerical features using histograms and box plots.
- Examined relationships among numerical variables using a correlation heatmap.
- Used count plots to explore categorical variables and customer churn patterns.

### 3. Handling Class Imbalance
Applied SMOTE (Synthetic Minority Over-sampling Technique) to address class imbalance in the training data. SMOTE was also incorporated into the cross-validation pipeline to avoid resampling the validation folds.

### 4. Model Building
Trained and compared the following classification algorithms:
- Decision Tree Classifier
- Random Forest Classifier
- XGBoost Classifier

### 5. Model Evaluation
Evaluated model performance using:
- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix

These metrics help assess how effectively the models identify customers who are likely to churn.

### 6. Model Saving and Prediction
Saved the trained Random Forest model using Python's Pickle module and loaded it for making predictions on new customer data.

## Results
The models were compared using cross-validation and test-set evaluation. The project achieved approximately **78% test accuracy** with the Random Forest model in the current implementation.

The results also highlight the importance of precision and recall when identifying customers at risk of leaving.

## Key Learnings
- Practical experience with the end-to-end machine learning workflow.
- Data cleaning, categorical encoding, and exploratory data analysis.
- Handling imbalanced datasets using SMOTE.
- Training and comparing multiple classification models.
- Evaluating classification performance beyond accuracy.
- Saving and loading a trained model for predictions.

## How to Run the Project
1. Clone or download this repository.
2. Install the required libraries:

   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn imbalanced-learn xgboost jupyter
   ```

3. Open the project notebook in Jupyter Notebook:

   ```bash
   jupyter notebook
   ```

4. Open `Customer Churn Project.ipynb` and run the cells in order.

## Future Improvements
- Improve categorical preprocessing and model performance.
- Perform hyperparameter tuning.
- Compare additional evaluation metrics and decision thresholds.
- Develop an interactive interface for customer churn predictions.

## Conclusion
This project demonstrates how machine learning classification techniques can be used to analyze customer behavior and predict churn. It provides practical experience in data analysis, model development, evaluation, and prediction.

**Author:** Muqeem Uddin
