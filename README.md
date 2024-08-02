# Airline Satisfaction using PySpark 
This project is dedicated to predicting airline traveler satisfaction by employing an end-to-end data processing and machine learning pipeline using PySpark and SparkML. 
It leverages the power of PySpark for data handling and Spark ML for building and evaluating predictive models. We explore and compare three machine learning algorithms: Random Forest, Linear Regression, and Gradient Boosted Trees. 
The project emphasizes robust data processing, model tuning, and visualization of results.

# Key Results
- Developed a predictive model with an accuracy exceeding 91%.
- Implemented and compared three different machine learning algorithms.
- Utilized visualizations such as accuracy curves across different thresholds and confusion matrices for each algorithm to interpret model performance.

# Requirements 
- PySpark(requires Apache Spark and Java on your local machine)
- Pandas, MatplotLib, NumPy, Seaborn
- Python 3.11

# Dataset 
The dataset used for this analysis is sourced from Kaggle, titled "Customer Satisfaction in Airline." 
It provides comprehensive data on various aspects of airline passengers' flight experiences. The dataset can be accessed here:
https://www.kaggle.com/datasets/yakhyojon/customer-satisfaction-in-airline.

# Process
1. Data Ingestion: Reading data using PySpark and converting it into a Spark DataFrame for further processing.
2. Data Preprocessing:
  - Conversion of string columns to integers and doubles for model compatibility.
  - Handling of null values by converting them to zeros.
  - Encoding of categorical columns.
  - Selection of relevant feature columns for the model.
3. Model Development:
  - Creation of three separate model pipelines for Random Forest, Logistic Regression, and Gradient Boosted Trees.
  - Splitting of data into 88% training and 12% testing sets.
  - Fitting model pipelines with training data.
4. Model Evaluation:
  - Testing different decision thresholds (ranging from 0.45 to 0.60) on the test dataset and comparing results.
  - Plotting the relationship between model accuracy and decision thresholds for each algorithm.
  - Generating and analyzing confusion matrices for the models at their highest accuracy thresholds.
