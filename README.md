 Credit Card Fraud Detection

📌 Overview
This project aims to detect fraudulent credit card transactions using Logistic Regression.  
The dataset is highly imbalanced, with only "492 fraud transactions" out of "284,807 total records".  
To overcome this, we balance the dataset by sampling an equal number of legitimate and fraudulent transactions.

 ⚙️ Features
- Data Cleaning:
  - No missing values in the dataset
  - Dataset has 31 columns: `Time`, `Amount`, 28 anonymized features (`V1`–`V28`), and `Class`
- Exploratory Analysis:
  - Fraud cases = 492  
  - Normal cases = 284,315
- Balancing:
  - Randomly sampled 492 legitimate transactions to match 492 fraud transactions
  - New balanced dataset: "984 transactions"(492 fraud, 492 legit)
- Model Training:
  - Logistic Regression used to classify transactions
  - Train-test split with stratification
- Results:
  - Accuracy on training data: ~94.5%
  - Accuracy on testing data: ~93.9%

 📂 Dataset
- File: `creditcard.csv`
- Source: [Kaggle – Credit Card Fraud Detection](https://www.kaggle.com/mlg-ulb/creditcardfraud)
- Columns:
  - `Time`: Seconds elapsed between transaction and first transaction in dataset
  - `V1`–`V28`: PCA-transformed features (originals hidden for privacy)
  - `Amount`: Transaction amount
  - `Class`: Target variable (`0 = Legit`, `1 = Fraud`)

