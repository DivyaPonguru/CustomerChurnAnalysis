About Dataset
Context
"Predict behavior to retain customers. You can analyze all relevant customer data and develop focused customer retention programs." 

Content
Each row represents a customer, each column contains customer’s attributes described on the column Metadata.

The data set includes information about:

Customers who left within the last month – the column is called Churn
Services that each customer has signed up for – phone, multiple lines, internet, online security, online backup, device protection, tech support, and streaming TV and movies
Customer account information – how long they’ve been a customer, contract, payment method, paperless billing, monthly charges, and total charges
Demographic info about customers – gender, age range, and if they have partners and dependents.

Project Overview
This project aims to predict customer churn in a telecom company. The analysis involves exploring customer data, cleaning the dataset, and applying machine learning models such as Logistic Regression and Random Forest to predict churn.

Libraries Used
This project uses several popular Python libraries to handle the data, perform analysis, and build machine learning models:

pip install pandas numpy matplotlib seaborn scikit-learn
Libraries:
pandas: Data handling and manipulation
numpy: Numerical computing
matplotlib & seaborn: Data visualization
scikit-learn: Machine learning models and evaluation

Steps Involved

1. Data Handling & Preprocessing
Import libraries: The required libraries for data handling, visualization, and machine learning are imported.
Load dataset: The dataset is loaded from a .csv file.
Data Info: Display dataset information (columns, data types, and null values).
Handle missing data: Convert columns to appropriate data types, and fill missing values with 0 where necessary.
Drop irrelevant columns: Remove columns that do not contribute to the analysis (e.g., customerID).
Encode categorical variables: Convert categorical variables to numeric values using LabelEncoder and the target variable (Churn) is encoded as 1 for "Yes" and 0 for "No".
Scale features: Standardize numeric features like tenure, MonthlyCharges, and TotalCharges using StandardScaler.

2. Exploratory Data Analysis (EDA)
Churn Distribution: Visualize the distribution of the target variable (Churn).
Correlation Heatmap: Display the correlation between features.
Monthly Charges vs. Churn: Visualize how MonthlyCharges affects churn.
Tenure vs. Churn: Analyze how customer tenure relates to churn using a histogram.

3. Machine Learning Models
Train-Test Split: Split the data into training and test sets using an 80-20 split.
Logistic Regression: Train a logistic regression model and evaluate its performance using accuracy and classification report.
Random Forest Classifier: Train a random forest model and evaluate its performance.

4. Model Evaluation
Compare model accuracy: Compare the accuracy of the Logistic Regression and Random Forest models.
Confusion Matrix: Visualize the confusion matrix for the Random Forest model to evaluate its performance.
