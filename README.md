📊 Data Pipeline Development: Iris Dataset (Colab)

🔍 Overview

This project demonstrates the end-to-end development of a basic data pipeline using the Iris dataset in Google Colab. It covers data loading, preprocessing, encoding, scaling, and exporting the cleaned dataset for further analysis or model training.


✅ Features

Upload and read CSV data in Google Colab

Basic EDA (data inspection, .info(), .describe(), .isnull())

Handle missing values

Encode categorical variables (LabelEncoder)

Scale numerical features (StandardScaler)

Split dataset into train-test sets

Save the processed dataset as CSV

Implemented a minimal sklearn Pipeline

🧠 Tech Stack

Python

Pandas

NumPy

Scikit-learn

Google Colab
❗ Problems Faced

FileNotFoundError while trying to load Iris.csv
Solution: Ensure the file is uploaded using files.upload() before calling pd.read_csv().

Label Encoding issues
Solution: Used LabelEncoder only on the 'Species' column after confirming it is categorical.

Scaling interfering with target column
Solution: Dropped the target column (Species) before scaling the features.

Google Colab file saving confusion
Solution: Used to_csv('processed_Iris.csv') to save and then download using Colab file browser.


📈 Future Enhancements

Add model training (Logistic Regression, Decision Tree, etc.)

Include cross-validation and performance metrics

Add visualization (e.g., seaborn pairplot)

Automate the pipeline with more steps using Pipeline

🙌 Acknowledgements

Thanks to the open-source community and the Iris Dataset from UCI ML Repository.
