# Credit Card Fraud Detection

This project demonstrates the process of detecting credit card fraud using a machine learning approach. It includes data preprocessing, handling class imbalance, and training a Decision Tree Classifier. The model is saved for future predictions.

## **Steps Performed**

1. **Dataset Loading**:
   - Read the dataset using `pandas`.
   - Explore the dataset for null values, duplicate entries, and basic statistics.

2. **Data Preprocessing**:
   - Remove duplicate data.
   - Normalize the 'Amount' column using `StandardScaler`.
   - Drop the 'Time' column.

3. **Handling Imbalanced Data**:
   - Use the Synthetic Minority Oversampling Technique (SMOTE) to handle class imbalance.

4. **Splitting the Data**:
   - Split the resampled data into training and testing sets using `train_test_split`.

5. **Model Training**:
   - Train a Decision Tree Classifier to predict fraud.
   - Evaluate the model's performance using a classification report.

6. **Model Saving**:
   - Save the trained model using `joblib` for future predictions.

## **Requirements**

- Python 3.8+
- Required Python libraries are listed in the `requirements.txt` file.

## **How to Run the Code**

1. Clone the repository:
   ```bash
   git clone https://github.com/your-repo-name/credit-card-fraud-detection.git
Install dependencies:
bash
Copy code
pip install -r requirements.txt
Place the creditcard.csv dataset in the same directory as the script.
Run the script:
bash
Copy code
python your_script_name.py
The model will be saved as credit_card_model in the current directory.
Dataset
The dataset creditcard.csv contains information about transactions made by credit cards in September 2013. The data includes:
Features representing transaction details.
A Class column indicating fraud (1) or non-fraud (0).
Acknowledgments
Dataset sourced from Kaggle Credit Card Fraud Detection Dataset.